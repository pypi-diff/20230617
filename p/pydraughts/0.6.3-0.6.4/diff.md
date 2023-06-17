# Comparing `tmp/pydraughts-0.6.3.tar.gz` & `tmp/pydraughts-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraughts-0.6.3.tar", last modified: Fri Jun  9 18:44:40 2023, max compression
+gzip compressed data, was "pydraughts-0.6.4.tar", last modified: Sat Jun 17 13:40:45 2023, max compression
```

## Comparing `pydraughts-0.6.3.tar` & `pydraughts-0.6.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.689990 pydraughts-0.6.3/
--rw-rw-rw-   0        0        0     1078 2023-06-09 18:40:53.000000 pydraughts-0.6.3/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-09 18:40:53.000000 pydraughts-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5389 2023-06-09 18:44:40.689990 pydraughts-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4147 2023-06-09 18:40:53.000000 pydraughts-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.193872 pydraughts-0.6.3/draughts/
--rw-rw-rw-   0        0        0    12623 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/PDN.py
--rw-rw-rw-   0        0        0      238 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.386915 pydraughts-0.6.3/draughts/ballot_files/
--rw-rw-rw-   0        0        0   350063 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/11_english.json
--rw-rw-rw-   0        0        0   191861 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/11_italian.json
--rw-rw-rw-   0        0        0    17530 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/150russian_and_brazilian.json
--rw-rw-rw-   0        0        0     5225 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/2move_english.json
--rw-rw-rw-   0        0        0    21036 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/3move_english.json
--rw-rw-rw-   0        0        0   104689 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/4move_english.json
--rw-rw-rw-   0        0        0   388564 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/5move_english.json
--rw-rw-rw-   0        0        0    95519 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/brazilian.json
--rw-rw-rw-   0        0        0    96764 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/russian.json
--rw-rw-rw-   0        0        0     2185 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballots.py
--rw-rw-rw-   0        0        0    11930 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/convert.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.458933 pydraughts-0.6.3/draughts/core/
--rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/__init__.py
--rw-rw-rw-   0        0        0     7019 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board.py
--rw-rw-rw-   0        0        0     2635 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board_initializer.py
--rw-rw-rw-   0        0        0     3406 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board_searcher.py
--rw-rw-rw-   0        0        0    35852 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/game.py
--rw-rw-rw-   0        0        0    19525 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/move.py
--rw-rw-rw-   0        0        0    28954 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/piece.py
--rw-rw-rw-   0        0        0    17684 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/variant.py
--rw-rw-rw-   0        0        0     1218 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engine.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.490941 pydraughts-0.6.3/draughts/engines/
--rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/__init__.py
--rw-rw-rw-   0        0        0     6447 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.582963 pydraughts-0.6.3/draughts/engines/checkerboard_extra/
--rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/__init__.py
--rw-rw-rw-   0        0        0     5506 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_64.py
--rw-rw-rw-   0        0        0     1133 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_client.py
--rw-rw-rw-   0        0        0     5091 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_server.py
--rw-rw-rw-   0        0        0     4405 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/get_checker_board.py
--rw-rw-rw-   0        0        0     7062 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.616973 pydraughts-0.6.3/draughts/engines/dxp_communication/
--rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/__init__.py
--rw-rw-rw-   0        0        0     8989 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_classes.py
--rw-rw-rw-   0        0        0     8796 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_communication.py
--rw-rw-rw-   0        0        0    14219 2023-06-07 12:42:58.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_run.py
--rw-rw-rw-   0        0        0    10797 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/hub.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.658983 pydraughts-0.6.3/other_licenses/
--rw-rw-rw-   0        0        0     1111 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/ImparaAI checkers LICENSE
--rw-rw-rw-   0        0        0     1075 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/akalverboer DXC100_draughts_client LICENSE
--rw-rw-rw-   0        0        0     1073 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/fishnet LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.685988 pydraughts-0.6.3/pydraughts.egg-info/
--rw-rw-rw-   0        0        0     5389 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2023-06-09 18:44:40.000000 pydraughts-0.6.3/pydraughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-09 18:40:53.000000 pydraughts-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0     1213 2023-06-09 18:44:40.695992 pydraughts-0.6.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.812527 pydraughts-0.6.4/
+-rw-rw-rw-   0        0        0     1078 2023-06-17 13:36:51.000000 pydraughts-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-17 13:36:51.000000 pydraughts-0.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5752 2023-06-17 13:40:45.813528 pydraughts-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-17 13:36:51.000000 pydraughts-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.575054 pydraughts-0.6.4/draughts/
+-rw-rw-rw-   0        0        0    13143 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/PDN.py
+-rw-rw-rw-   0        0        0      205 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.640830 pydraughts-0.6.4/draughts/ballot_files/
+-rw-rw-rw-   0        0        0   350063 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/11_english.json
+-rw-rw-rw-   0        0        0   191861 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/11_italian.json
+-rw-rw-rw-   0        0        0    17530 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/150russian_and_brazilian.json
+-rw-rw-rw-   0        0        0     5225 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/2move_english.json
+-rw-rw-rw-   0        0        0    21036 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/3move_english.json
+-rw-rw-rw-   0        0        0   104689 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/4move_english.json
+-rw-rw-rw-   0        0        0   388564 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/5move_english.json
+-rw-rw-rw-   0        0        0    95519 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/brazilian.json
+-rw-rw-rw-   0        0        0    96764 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballot_files/russian.json
+-rw-rw-rw-   0        0        0     2208 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/ballots.py
+-rw-rw-rw-   0        0        0    12188 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/convert.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.694215 pydraughts-0.6.4/draughts/core/
+-rw-rw-rw-   0        0        0        0 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/__init__.py
+-rw-rw-rw-   0        0        0     7155 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/board.py
+-rw-rw-rw-   0        0        0     2662 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/board_initializer.py
+-rw-rw-rw-   0        0        0     3559 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/board_searcher.py
+-rw-rw-rw-   0        0        0    36292 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/game.py
+-rw-rw-rw-   0        0        0    18975 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/move.py
+-rw-rw-rw-   0        0        0    29175 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/piece.py
+-rw-rw-rw-   0        0        0    18729 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/core/variant.py
+-rw-rw-rw-   0        0        0     1252 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.713051 pydraughts-0.6.4/draughts/engines/
+-rw-rw-rw-   0        0        0        0 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/__init__.py
+-rw-rw-rw-   0        0        0     6637 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.740920 pydraughts-0.6.4/draughts/engines/checkerboard_extra/
+-rw-rw-rw-   0        0        0        0 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard_extra/__init__.py
+-rw-rw-rw-   0        0        0     5769 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_64.py
+-rw-rw-rw-   0        0        0     1433 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_client.py
+-rw-rw-rw-   0        0        0     5346 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_server.py
+-rw-rw-rw-   0        0        0     4405 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/checkerboard_extra/get_checker_board.py
+-rw-rw-rw-   0        0        0     8960 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/dxp.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.764430 pydraughts-0.6.4/draughts/engines/dxp_communication/
+-rw-rw-rw-   0        0        0        0 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/dxp_communication/__init__.py
+-rw-rw-rw-   0        0        0     9121 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/dxp_communication/dxp_classes.py
+-rw-rw-rw-   0        0        0     9906 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/dxp_communication/dxp_communication.py
+-rw-rw-rw-   0        0        0    10884 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/engines/hub.py
+-rw-rw-rw-   0        0        0    10165 2023-06-17 13:36:51.000000 pydraughts-0.6.4/draughts/tournament.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.780440 pydraughts-0.6.4/other_licenses/
+-rw-rw-rw-   0        0        0     1111 2023-06-17 13:36:51.000000 pydraughts-0.6.4/other_licenses/ImparaAI checkers LICENSE
+-rw-rw-rw-   0        0        0     1075 2023-06-17 13:36:51.000000 pydraughts-0.6.4/other_licenses/akalverboer DXC100_draughts_client LICENSE
+-rw-rw-rw-   0        0        0     1073 2023-06-17 13:36:51.000000 pydraughts-0.6.4/other_licenses/fishnet LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 13:40:45.808528 pydraughts-0.6.4/pydraughts.egg-info/
+-rw-rw-rw-   0        0        0     5752 2023-06-17 13:40:45.000000 pydraughts-0.6.4/pydraughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1571 2023-06-17 13:40:45.000000 pydraughts-0.6.4/pydraughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:40:45.000000 pydraughts-0.6.4/pydraughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-17 13:40:45.000000 pydraughts-0.6.4/pydraughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 13:40:45.000000 pydraughts-0.6.4/pydraughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-17 13:36:51.000000 pydraughts-0.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1213 2023-06-17 13:40:45.817532 pydraughts-0.6.4/setup.cfg
```

### Comparing `pydraughts-0.6.3/LICENSE` & `pydraughts-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/PKG-INFO` & `pydraughts-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.3
+Version: 0.6.4
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
 Author: Ioannis Pantidis
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -139,14 +139,25 @@
 * Get a ballot
 ```python
 from draughts.ballots import Ballots
 ballots = Ballots('english')
 ballot1 = ballots.get_ballot()
 ballot2 = ballots.get_ballot()
 ```
+* Run tournaments
+```python
+from draughts.tournament import RoundRobin
+player1 = (["scan.exe", "hub"], "hub", {})
+player2 = ("kr_hub.exe", "hub", {})
+players = [player1, player2]
+tournament = RoundRobin("tournament.pdn", players, start_time=20, increment=0.2, games_per_pair=4)
+scores = tournament.play()
+print(scores)
+tournament.print_standings()
+```
 
 ## Acknowledgements
 Thanks to [fishnet](https://github.com/lichess-org/fishnet/tree/ebd2a5e16d37135509cbfbff9998e0b798866ef5) which was modified to add support for Hub engines. Thanks to [akalverboer](https://github.com/akalverboer) for their [DXC100_draughts_client](https://github.com/akalverboer/DXC100_draughts_client) which was modified to add support for DXP engines.
 
 ## License
 pydraughts is licensed under The MIT License. Check out `LICENSE` for the full text.
 The licenses of the other projects that pydraughts uses are in the `other_licenses` folder.
```

### Comparing `pydraughts-0.6.3/README.md` & `pydraughts-0.6.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -116,14 +116,25 @@
 * Get a ballot
 ```python
 from draughts.ballots import Ballots
 ballots = Ballots('english')
 ballot1 = ballots.get_ballot()
 ballot2 = ballots.get_ballot()
 ```
+* Run tournaments
+```python
+from draughts.tournament import RoundRobin
+player1 = (["scan.exe", "hub"], "hub", {})
+player2 = ("kr_hub.exe", "hub", {})
+players = [player1, player2]
+tournament = RoundRobin("tournament.pdn", players, start_time=20, increment=0.2, games_per_pair=4)
+scores = tournament.play()
+print(scores)
+tournament.print_standings()
+```
 
 ## Acknowledgements
 Thanks to [fishnet](https://github.com/lichess-org/fishnet/tree/ebd2a5e16d37135509cbfbff9998e0b798866ef5) which was modified to add support for Hub engines. Thanks to [akalverboer](https://github.com/akalverboer) for their [DXC100_draughts_client](https://github.com/akalverboer/DXC100_draughts_client) which was modified to add support for DXP engines.
 
 ## License
 pydraughts is licensed under The MIT License. Check out `LICENSE` for the full text.
 The licenses of the other projects that pydraughts uses are in the `other_licenses` folder.
```

### Comparing `pydraughts-0.6.3/draughts/PDN.py` & `pydraughts-0.6.4/draughts/PDN.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 import string
-from functools import reduce
 from draughts.convert import fen_to_variant
 from draughts import Board, Move
 from typing import List, Optional, Dict, Union
 
 
 class _PDNGame:
     """Read one PDN game."""
     def __init__(self, pdn_text: str) -> None:
-        self.values_to_variant = {20: "standard", 21: "english", 22: "italian", 23: "american pool", 24: "spanish", 25: "russian", 26: "brazilian", 27: "canadian", 28: "portuguese", 29: "czech", 30: "turkish", 31: "thai", 40: "frisian", 41: "spantsiretti"}
+        self.values_to_variant = {20: "standard", 21: "english", 22: "italian", 23: "american pool", 24: "spanish",
+                                  25: "russian", 26: "brazilian", 27: "canadian", 28: "portuguese", 29: "czech",
+                                  30: "turkish", 31: "thai", 40: "frisian", 41: "spantsiretti"}
         self.tags: Dict[str, str] = {}
         self.moves: List[str] = []
         self.variant: Optional[str] = None
         self.notation: Optional[int] = None
         self.notation_type: Optional[str] = None
         self.game_ending = '*'
         self.pdn_text = pdn_text
@@ -57,21 +58,21 @@
         rest_of_games += lines[last_tag_line + 1 + last_move_line + 1:]
 
         str_moves = " ".join(move_lines)
 
         # Changes to the PDN.
 
         # From https://stackoverflow.com/a/37538815/10014873
-        def remove_text_between_parens(text):
+        def remove_text_between_parens(text: str) -> str:
             n = 1  # Run at least once.
             while n:
                 text, n = re.subn(r'\([^()]*\)', '', text)  # Remove non-nested/flat balanced parts.
             return text
 
-        def remove_text_between_brackets(text):
+        def remove_text_between_brackets(text: str) -> str:
             n = 1  # Run at least once.
             while n:
                 text, n = re.subn(r'{[^{}]*}', '', text)  # Remove non-nested/flat balanced parts.
             return text
 
         str_moves = remove_text_between_parens(str_moves)
         str_moves = remove_text_between_brackets(str_moves)
@@ -85,27 +86,34 @@
         str_moves = str_moves.replace('- ', '-')
         str_moves = str_moves.replace('x ', 'x')
         str_moves = str_moves.replace(': ', ':')
 
         move_numbers = re.findall(r"\d+\.", str_moves)
         double_numbers = list(set(filter(lambda move: move_numbers.count(move) >= 2, move_numbers)))
         for move_number in double_numbers:
-            str_moves = str_moves[:str_moves.index(move_number) + len(move_number)] + str_moves[str_moves.index(move_number) + len(move_number):].replace(move_number, "")
+            str_moves = (str_moves[:str_moves.index(move_number) + len(move_number)] +
+                         str_moves[str_moves.index(move_number) + len(move_number):].replace(move_number, ""))
 
         moves = str_moves.split(".")[1:]
         if not moves:
             return
         starts = self.tags.get('FEN', 'W')
         if starts.startswith('W'):
-            moves = list(reduce(lambda x, y: x + y.split()[:2], moves, []))
+            clean_moves = []
+            list_moves = [move.split()[:2] for move in moves]
+            for move in list_moves:
+                clean_moves.extend(move)
         else:
-            moves = [moves[0].split()[0]] + list(reduce(lambda x, y: x + y.split()[:2], moves[1:], []))
+            clean_moves = [moves[0].split()[0]]
+            list_moves = [[moves[0].split()[0]]] + [move.split()[:2] for move in moves[1:]]
+            for move in list_moves:
+                clean_moves.extend(move)
         results = ["1-0", "1/2-1/2", "0-1", "2-0", "1-1", "0-2", "0-0", "*"]
-        moves = moves[:-1] if moves[-1] in results else moves
-        self.moves = moves
+        clean_moves = clean_moves[:-1] if clean_moves[-1] in results else clean_moves
+        self.moves = clean_moves
 
         if "GameType" in self.tags:
             game_type = self.tags["GameType"]
             values = game_type.split(',')
             variant_number = int(values[0])
             self.variant = self.values_to_variant.get(variant_number, None)
             if len(values) == 6:
@@ -145,29 +153,30 @@
         """Get the rest of the games."""
         # This class only reads the first game. You can get the rest with this function.
         return '\n'.join(self._rest_of_games)
 
 
 class PDNReader:
     """Read PDN games."""
-    def __init__(self, pdn_text: Optional[str] = None, filename: Optional[str] = None, encodings: Union[List[str], str, None] = None) -> None:
-        assert pdn_text or filename
+    def __init__(self, pdn_text: Optional[str] = None, filename: Optional[str] = None,
+                 encodings: Union[List[str], str, None] = None) -> None:
         if encodings is None:
             encodings = ['utf8', 'ISO 8859/1']
         if type(encodings) == str:
             encodings = [encodings]
-        if not pdn_text:
+        if filename:
             pdn_text = ''
             for encoding in encodings:
                 try:
                     with open(filename, encoding=encoding) as pdn_file:
                         pdn_text = pdn_file.read()
                     break
                 except Exception:
                     pass
+        assert pdn_text is not None
         self.pdn_text = pdn_text
         self.pdn_text = re.sub('\n +', '\n', self.pdn_text)
         self.pdn_text = re.sub('\n\n+', '\n\n', self.pdn_text)
         self.games = []
         game = _PDNGame(self.pdn_text)
         self.games.append(game)
         more_games = game._get_rest_of_games()
@@ -175,34 +184,40 @@
             game = _PDNGame(more_games)
             self.games.append(game)
             more_games = game._get_rest_of_games()
 
 
 class PDNWriter:
     """Write a game to a file."""
-    VARIANT_TO_GAMETYPE = {'standard': 20, 'english': 21, 'italian': 22, 'russian': 25, 'brazilian': 26, 'turkish': 30, 'frisian': 40, 'frysk!': 40}
-    SHORT_TO_LONG_GAMETYPE = {'20': '20,W,10,10,N2,0', '21': '21,B,8,8,N1,0', '22': '22,W,8,8,N2,1', '25': '25,W,8,8,A0,0', '26': '26,W,8,8,A0,0', '30': '30,W,8,8,A0,0', '40': '40,W,10,10,N2,0'}
-
-    def __init__(self, filename: str, board: Optional[Board] = None, moves: Optional[List[Union[str, Move]]] = None, variant: Optional[str] = None, starting_fen: Optional[str] = None, tags: Optional[Dict[str, Union[str, int]]] = None, game_ending: str = '*', replay_moves_from_board: bool = True, file_encoding: str = 'utf8', file_mode: str = 'a') -> None:
+    VARIANT_TO_GAMETYPE = {'standard': 20, 'english': 21, 'italian': 22, 'russian': 25, 'brazilian': 26, 'turkish': 30,
+                           'frisian': 40, 'frysk!': 40}
+    SHORT_TO_LONG_GAMETYPE = {'20': '20,W,10,10,N2,0', '21': '21,B,8,8,N1,0', '22': '22,W,8,8,N2,1',
+                              '25': '25,W,8,8,A0,0', '26': '26,W,8,8,A0,0', '30': '30,W,8,8,A0,0', '40': '40,W,10,10,N2,0'}
+
+    def __init__(self, filename: str, board: Optional[Board] = None, moves: Union[List[str], List[Move], None] = None,
+                 variant: Optional[str] = None, starting_fen: Optional[str] = None,
+                 tags: Optional[Dict[str, Union[str, int]]] = None, game_ending: str = '*',
+                 replay_moves_from_board: bool = True, file_encoding: str = 'utf8', file_mode: str = 'a') -> None:
         """
         :param replay_moves_from_board: The already saved pdn_move in move_stack may be wrong because it is pseudolegal
         and doesn't account for ambiguous moves. If replay_moves_from_board is enabled, it will replay all the moves to
         find the correct representation of them.
         """
         assert board or moves is not None
         self.pdn_text = ''
         self.notation_type: Optional[str] = None
         self.notation: Optional[int] = None
 
         self.board = board
+        self.moves: Union[List[str], List[Move]]
         if self.board:
             self.moves = self.board.move_stack
             self.variant = self.board.variant
             self.starting_fen = self.board.initial_fen
-            self.tags = {}
+            self.tags = tags or {}
         else:
             self.moves = moves
             self.variant = variant or 'standard'
             self.starting_fen = starting_fen or self._startpos_to_fen()
             self.tags = tags or {}
         self.game_ending = game_ending
```

### Comparing `pydraughts-0.6.3/draughts/ballot_files/11_english.json` & `pydraughts-0.6.4/draughts/ballot_files/11_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/11_italian.json` & `pydraughts-0.6.4/draughts/ballot_files/11_italian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/150russian_and_brazilian.json` & `pydraughts-0.6.4/draughts/ballot_files/150russian_and_brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/2move_english.json` & `pydraughts-0.6.4/draughts/ballot_files/2move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/3move_english.json` & `pydraughts-0.6.4/draughts/ballot_files/3move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/4move_english.json` & `pydraughts-0.6.4/draughts/ballot_files/4move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/5move_english.json` & `pydraughts-0.6.4/draughts/ballot_files/5move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/brazilian.json` & `pydraughts-0.6.4/draughts/ballot_files/brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballot_files/russian.json` & `pydraughts-0.6.4/draughts/ballot_files/russian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/ballots.py` & `pydraughts-0.6.4/draughts/ballots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# 11 english, 11 italian, 4 move english and 5 move english ballots are from Ed Gilbert (http://edgilbert.org/Checkers/KingsRow.htm).
+# 11 english, 11 italian, 4 move english and 5 move english ballots are from
+# Ed Gilbert (http://edgilbert.org/Checkers/KingsRow.htm).
+
 import random
 import json
 import os
 from typing import Tuple, List, Dict
 
 
 class Ballots:
-    def __init__(self, variant: str, moves: int = 3, eleven_pieces: bool = False, basic_positions: bool = False, include_lost_games: bool = False) -> None:
+    def __init__(self, variant: str, moves: int = 3, eleven_pieces: bool = False, basic_positions: bool = False,
+                 include_lost_games: bool = False) -> None:
         self.variant = variant
         self.moves = moves
         self.eleven_pieces = eleven_pieces
         self.basic_positions = basic_positions
         self.include_lost_games = include_lost_games
         self.filename = self._find_file()
         self.positions, self.keys = self.open_file()
```

### Comparing `pydraughts-0.6.3/draughts/convert.py` & `pydraughts-0.6.4/draughts/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     correct_seperator = ''
     for separator in separators:
         split_move = internal_move.split(separator)
         if split_move[0] != internal_move:
             correct_seperator = separator
             break
     int_move_parts = list(map(int, split_move))
-    variant_to_notation = {'standard': 2, 'english': 1, 'italian': 2, 'russian': 0, 'brazilian': 0, 'turkish': 0, 'frisian': 2, 'frysk!': 2, 'antidraughts': 2, 'breakthrough': 2}
+    variant_to_notation = {'standard': 2, 'english': 1, 'italian': 2, 'russian': 0, 'brazilian': 0, 'turkish': 0,
+                           'frisian': 2, 'frysk!': 2, 'antidraughts': 2, 'breakthrough': 2}
     if notation is None:
         notation = variant_to_notation.get(variant, 2)
 
     def reverse_column(split_int_move: List[int]) -> List[int]:
         per_row = _get_squares(variant)[1]
         for index, square in enumerate(split_int_move):
             square_in_row = square % per_row
@@ -64,15 +65,16 @@
     else:  # notation == 3
         rotated_move = reverse_column(int_move_parts)
 
     rotated_str_move = list(map(str, rotated_move))
     return correct_seperator.join(rotated_str_move)
 
 
-def _algebraic_to_number(algebraic_move: str, squares_per_letter: Optional[int] = None, variant: Optional[str] = None, every_other_square: Optional[bool] = None) -> str:
+def _algebraic_to_number(algebraic_move: str, squares_per_letter: Optional[int] = None, variant: Optional[str] = None,
+                         every_other_square: Optional[bool] = None) -> str:
     """Convert an algebraic move to a numeric move."""
     if every_other_square is None:
         if variant == 'turkish':
             every_other_square = False
         else:
             every_other_square = True
     algebraic_notation = algebraic_move[0] in string.ascii_letters
@@ -112,15 +114,16 @@
     if not algebraic_notation:
         return int(square)
     if not every_other_square:
         return (int(square[1]) - 1) * squares_per_letter + string.ascii_lowercase.index(square[0]) + 1
     return (int(square[1]) - 1) * squares_per_letter + ceil(string.ascii_lowercase.index(square[0]) // 2) + 1
 
 
-def _number_to_algebraic(number_move: str, width: Optional[int] = None, variant: Optional[str] = None, every_other_square: Optional[bool] = None) -> str:
+def _number_to_algebraic(number_move: str, width: Optional[int] = None, variant: Optional[str] = None,
+                         every_other_square: Optional[bool] = None) -> str:
     """Convert a numeric move to an algebraic move."""
     if every_other_square is None:
         every_other_square = _get_squares(variant)[3]
     algebraic_notation = number_move[0] in string.ascii_letters
     if algebraic_notation:
         return number_move
     if width is None:
@@ -151,15 +154,16 @@
     column = (int_square - 1) % width
     if every_other_square:
         column *= 2
         column += 1 if row % 2 == 1 else 0
     return string.ascii_lowercase[column] + str(row + 1)
 
 
-def _change_fen_from_variant(li_fen: str, notation: Optional[int] = None, squares_per_letter: int = 5, every_other_square: bool = True, variant: Optional[str] = None) -> str:
+def _change_fen_from_variant(li_fen: str, notation: Optional[int] = None, squares_per_letter: int = 5,
+                             every_other_square: bool = True, variant: Optional[str] = None) -> str:
     """Convert an internal fen to the correct fen for the variant."""
     if variant:
         _, _, squares_per_letter, every_other_square = _get_squares(variant)
 
     fen = li_fen.split(':')
     if len(fen) < 3:
         return li_fen
@@ -173,41 +177,49 @@
     for white_piece in white_pieces:
         if '-' in white_piece:
             start_end = white_piece.split('-')
             add_for_king = ''
             if start_end[0][0] == 'K':
                 add_for_king = 'K'
                 start_end[0] = start_end[0][1:]
-            start, end = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square), _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
+            start = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square)
+            end = _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
             for number in range(start, end + 1):
                 white_pieces_remove_hyphen.append(add_for_king + _rotate_move(str(number), notation=notation, variant=variant))
         else:
             add_for_king = ''
             if white_piece[0] == 'K':
                 add_for_king = 'K'
                 white_piece = white_piece[1:]
-            white_pieces_remove_hyphen.append(add_for_king + _rotate_move(str(_algebraic_to_numeric_square(white_piece, squares_per_letter, every_other_square)), notation=notation, variant=variant))
+            white_pieces_remove_hyphen.append(
+                add_for_king + _rotate_move(
+                    str(_algebraic_to_numeric_square(white_piece, squares_per_letter, every_other_square)),
+                    notation=notation, variant=variant))
 
     black_pieces_remove_hyphen = []
     for black_piece in black_pieces:
         if '-' in black_piece:
             start_end = black_piece.split('-')
             add_for_king = ''
             if start_end[0][0] == 'K':
                 add_for_king = 'K'
                 start_end[0] = start_end[0][1:]
-            start, end = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square), _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
+            start = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square)
+            end = _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
             for number in range(start, end + 1):
                 black_pieces_remove_hyphen.append(add_for_king + _rotate_move(str(number), notation=notation, variant=variant))
         else:
             add_for_king = ''
             if black_piece[0] == 'K':
                 add_for_king = 'K'
                 black_piece = black_piece[1:]
-            black_pieces_remove_hyphen.append(add_for_king + _rotate_move(str(_algebraic_to_numeric_square(black_piece, squares_per_letter, every_other_square)), notation=notation, variant=variant))
+            black_pieces_remove_hyphen.append(
+                add_for_king + _rotate_move(
+                    str(_algebraic_to_numeric_square(black_piece, squares_per_letter, every_other_square)),
+                    notation=notation, variant=variant))
 
     # Because in english black starts.
     white_starts = variant not in ['english']
     if not white_starts:
         white_pieces_remove_hyphen, black_pieces_remove_hyphen = black_pieces_remove_hyphen, white_pieces_remove_hyphen
         starts = 'W' if starts == 'B' else 'B'
```

### Comparing `pydraughts-0.6.3/draughts/core/board.py` & `pydraughts-0.6.4/draughts/core/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,35 +49,39 @@
         self.pieces_promote_and_stop_capturing = self.variant in ['english', 'italian']
         self.pieces_promote_and_continue_capturing = self.variant in ['russian']
 
     def count_movable_player_pieces(self, player_number: int = 1, captures: Optional[List[int]] = None) -> int:
         """Count the pieces of one player that can be moved."""
         if captures is None:
             captures = []
-        return reduce((lambda count, piece: count + (1 if piece.is_movable(captures) else 0)), self.searcher.get_pieces_by_player(player_number), 0)
+        return reduce((lambda count, piece: count + (1 if piece.is_movable(captures) else 0)),
+                      self.searcher.get_pieces_by_player(player_number), 0)
 
     def get_possible_moves(self, captures: List[int]) -> List[List[int]]:
         """Get all possible moves."""
         capture_moves = self.get_possible_capture_moves(captures)
 
         return capture_moves if capture_moves else self.get_possible_positional_moves()
 
     def get_possible_capture_moves(self, captures: List[int]) -> List[List[int]]:
         """Get all possible capture moves (not positional moves)."""
-        return reduce((lambda moves, piece: moves + piece.get_possible_capture_moves(captures)), self.searcher.get_pieces_in_play(), [])
+        return reduce((lambda moves, piece: moves + piece.get_possible_capture_moves(captures)),
+                      self.searcher.get_pieces_in_play(), [])
 
     def get_possible_positional_moves(self) -> List[List[int]]:
         """Get all possible positional moves (not capture moves)."""
-        return reduce((lambda moves, piece: moves + piece.get_possible_positional_moves()), self.searcher.get_pieces_in_play(), [])
+        return reduce((lambda moves, piece: moves + piece.get_possible_positional_moves()),
+                      self.searcher.get_pieces_in_play(), [])
 
     def position_is_open(self, position: int) -> bool:
         """Get if the position is open (a piece is not in the given square)."""
         return position in self.searcher.open_positions
 
-    def create_new_board_from_move(self, move: List[int], move_number: int, captures: List[int]) -> Tuple[Board, Optional[int]]:
+    def create_new_board_from_move(self, move: List[int], move_number: int, captures: List[int]
+                                   ) -> Tuple[Board, Optional[int]]:
         """Create a new board and play the move given."""
         new_board = pickle.loads(pickle.dumps(self, -1))  # A lot faster that deepcopy.
         enemy_position = None
 
         if move in self.get_possible_capture_moves(captures):
             enemy_position = new_board.perform_capture_move(move, move_number, captures)
         else:
@@ -107,19 +111,21 @@
         enemy_piece.capture()
         self.move_piece(piece, move[1], move_number)
         if not originally_was_king and piece.king and self.pieces_promote_and_stop_capturing:
             further_capture_moves_for_piece = []
         elif not originally_was_king and not self.pieces_promote_and_continue_capturing:
             was_king = piece.king
             piece.king = False
-            further_capture_moves_for_piece = [capture_move for capture_move in self.get_possible_capture_moves(captures + [enemy_position]) if move[1] == capture_move[0]]
+            further_capture_moves_for_piece = [capture_move for capture_move in self.get_possible_capture_moves(
+                captures + [enemy_position]) if move[1] == capture_move[0]]
             if not further_capture_moves_for_piece and was_king:
                 piece.king = True
         else:
-            further_capture_moves_for_piece = [capture_move for capture_move in self.get_possible_capture_moves(captures + [enemy_position]) if move[1] == capture_move[0]]
+            further_capture_moves_for_piece = [capture_move for capture_move in self.get_possible_capture_moves(
+                captures + [enemy_position]) if move[1] == capture_move[0]]
 
         if further_capture_moves_for_piece:
             self.piece_requiring_further_capture_moves = self.searcher.get_piece_by_position(move[1])
         else:
             self.piece_requiring_further_capture_moves = None
             self.switch_turn()
         return enemy_position
```

### Comparing `pydraughts-0.6.3/draughts/core/board_initializer.py` & `pydraughts-0.6.4/draughts/core/board_initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             player_starting_positions = {
                 1: list(range(1, starting_piece_count + 1)),
                 2: list(range(self.board.position_count - starting_piece_count + 1, self.board.position_count + 1))
             }
 
             for key, row in self.board.position_layout.items():
                 for key, position in row.items():
-                    player_number = 1 if position in player_starting_positions[1] else 2 if position in player_starting_positions[2] else None
+                    player_number = 1 if position in player_starting_positions[1] else (
+                        2 if position in player_starting_positions[2] else None)
 
                     if player_number:
                         pieces.append(self.create_piece(player_number, position))
 
         self.board.pieces = pieces
 
     def create_piece(self, player_number: int, position: int) -> Piece:
```

### Comparing `pydraughts-0.6.3/draughts/core/board_searcher.py` & `pydraughts-0.6.4/draughts/core/board_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,37 @@
         self.build_open_positions()
         self.build_player_positions()
         self.build_player_pieces()
         self.build_position_pieces()
 
     def build_filled_positions(self) -> None:
         """Find the filled positions (squares which have a piece)."""
-        self.filled_positions = reduce((lambda open_positions, piece: open_positions + [piece.position]), self.uncaptured_pieces, [])
+        self.filled_positions = reduce((lambda open_positions, piece: open_positions + [piece.position]),
+                                       self.uncaptured_pieces, [])
 
     def build_open_positions(self) -> None:
         """Find the open positions (empty squares)."""
         self.open_positions = list(set(range(1, self.board.position_count + 1)).difference(self.filled_positions))
 
     def build_player_positions(self) -> None:
         """Find the positions where each player has a piece."""
         self.player_positions = {
-            1: reduce((lambda positions, piece: positions + ([piece.position] if piece.player == BLACK else [])), self.uncaptured_pieces, []),
-            2: reduce((lambda positions, piece: positions + ([piece.position] if piece.player == WHITE else [])), self.uncaptured_pieces, [])
+            1: reduce((lambda positions, piece: positions + ([piece.position] if piece.player == BLACK else [])),
+                      self.uncaptured_pieces, []),
+            2: reduce((lambda positions, piece: positions + ([piece.position] if piece.player == WHITE else [])),
+                      self.uncaptured_pieces, [])
         }
 
     def build_player_pieces(self) -> None:
         """Find all the pieces of both players."""
         self.player_pieces = {
-            BLACK: reduce((lambda pieces, piece: pieces + ([piece] if piece.player == BLACK else [])), self.uncaptured_pieces, []),
-            WHITE: reduce((lambda pieces, piece: pieces + ([piece] if piece.player == WHITE else [])), self.uncaptured_pieces, [])
+            BLACK: reduce((lambda pieces, piece: pieces + ([piece] if piece.player == BLACK else [])),
+                          self.uncaptured_pieces, []),
+            WHITE: reduce((lambda pieces, piece: pieces + ([piece] if piece.player == WHITE else [])),
+                          self.uncaptured_pieces, [])
         }
 
     def build_position_pieces(self) -> None:
         """Make a dict where the key is the square and the value is the piece in this square."""
         self.position_pieces = {piece.position: piece for piece in self.uncaptured_pieces}
 
     def get_pieces_by_player(self, player_number: int) -> List[Piece]:
@@ -61,12 +66,13 @@
 
     def get_pieces_in_play(self) -> List[Piece]:
         """
         Get pieces in play. They are: All the pieces of the player playing now except when a piece is
         in the middle of a multi-capture, so it has already captured one or more pieces, but it can capture more,
         where we only return the piece that is in the middle of the multi-capture.
         """
-        return self.player_pieces[self.board.player_turn] if not self.board.piece_requiring_further_capture_moves else [self.board.piece_requiring_further_capture_moves]
+        return (self.player_pieces[self.board.player_turn] if not self.board.piece_requiring_further_capture_moves else
+                [self.board.piece_requiring_further_capture_moves])
 
     def get_piece_by_position(self, position: int) -> Piece:
         """Get the piece given its position."""
         return self.position_pieces[position]
```

### Comparing `pydraughts-0.6.3/draughts/core/game.py` & `pydraughts-0.6.4/draughts/core/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         self.last_non_reversible_fen_history = [self.last_non_reversible_fen]
         self.moves_since_last_capture_history = [self.moves_since_last_capture]
         self.consecutive_noncapture_king_moves_history = [self.consecutive_noncapture_king_moves]
 
     def copy(self) -> Game:
         """Copy the board (transfers all data)."""
         # At least 6 times faster than deepcopy.
-        return pickle.loads(pickle.dumps(self, -1))
+        copy_game: Game = pickle.loads(pickle.dumps(self, -1))
+        return copy_game
 
     def copy_fast(self) -> Game:
         """Copy the board (doesn't transfer all the data but is faster)."""
         # More than 10x faster than .copy() but it doesn't transfer all the data.
         game = Game(self.variant, self.get_fen())
         game._not_added_move = self._not_added_move.copy()
         game._not_added_capture = self._not_added_capture.copy()
@@ -94,15 +95,15 @@
 
                 self.last_non_reversible_fen_history.pop()
                 self.moves_since_last_capture_history.pop()
                 self.consecutive_noncapture_king_moves_history.pop()
 
             self.board = Board(self.variant, self.fens[-1])
 
-    def move(self, move: List[int], return_captured: bool = False, include_pdn=False) -> Union[Game, Tuple[Game, Optional[int]]]:
+    def move(self, move: List[int], include_pdn: bool = False) -> Tuple[Game, Optional[int]]:
         """Make a move. Plays only one jump in case of a multi-capture and not the whole sequence."""
         # [0, 0] is a null move.
         is_null_move = move == [0, 0]
         if move not in self.get_possible_moves() and not is_null_move:
             raise ValueError('The provided move is not possible')
         turn = self.whose_turn()
         was_king = False
@@ -112,27 +113,29 @@
             self.board.switch_turn()
             enemy_position = None
         else:
             was_king = self.board.searcher.get_piece_by_position(move[0]).king
             self.board, enemy_position = self.board.push_move(move, len(self.move_stack) + 1, self._not_added_capture)
         self.moves.append(move)
 
-        if self.whose_turn() == turn:
+        if self.whose_turn() == turn and enemy_position is not None:  # `enemy_position is not None` is there only for mypy.
             self._not_added_move.append(move)
             self._not_added_capture.append(enemy_position)
         else:
-            captures = self._not_added_capture + [enemy_position]
-            if captures[0] is None:
-                captures = []
+            captures = []
+            if enemy_position:
+                captures = self._not_added_capture + [enemy_position]
             move_to_add_board = self._not_added_move + [move]
-            move_to_add_hub = self.make_len_2(move_to_add_board[0][0]) + self.make_len_2(move_to_add_board[-1][1]) + self.sort_captures(captures)
+            move_to_add_hub = self.make_len_2(move_to_add_board[0][0]) + self.make_len_2(
+                move_to_add_board[-1][1]) + self.sort_captures(captures)
             if include_pdn:
                 move_to_add = StandardMove(board=old_board, board_move=move_to_add_board)
             else:
-                move_to_add = StandardMove(board_move=move_to_add_board, hub_position_move=move_to_add_hub, has_captures=bool(captures), hub_to_pdn_pseudolegal=True)
+                move_to_add = StandardMove(board_move=move_to_add_board, hub_position_move=move_to_add_hub,
+                                           has_captures=bool(captures), hub_to_pdn_pseudolegal=True)
             self.move_stack.append(move_to_add)
             self.capture_stack.append(captures)
             self._not_added_move = []
             self._not_added_capture = []
 
             self.moves_since_last_capture = 0 if self.board.previous_move_was_capture else self.moves_since_last_capture + 1
             if was_king and not captures:
@@ -143,31 +146,22 @@
                 self.reversible_moves = []
                 self.consecutive_noncapture_king_moves = 0
             self.last_non_reversible_fen_history.append(self.last_non_reversible_fen)
             self.moves_since_last_capture_history.append(self.moves_since_last_capture)
             self.consecutive_noncapture_king_moves_history.append(self.consecutive_noncapture_king_moves)
             self.fens.append(self.get_fen())
 
-        if return_captured:
-            return self, enemy_position
-        else:
-            return self
+        return self, enemy_position
 
-    def push(self, move: Union[List[List[int]], List[int]], return_captured: bool = False, include_pdn=False) -> Union[Game, Tuple[Game, List[int]]]:
+    def push(self, move: List[List[int]], include_pdn: bool = False) -> Tuple[Game, List[Optional[int]]]:
         """Make a move. Plays the whole move sequence in case of a capture."""
-        if type(move[0]) == int:
-            move = [move]
         enemy_positions = []
         for move_part in move:
-            enemy_positions.append(self.move(move_part, return_captured, include_pdn))
-        if return_captured:
-            enemy_positions = list(map(lambda game_enemy_position: game_enemy_position[1], enemy_positions))
-            return self, enemy_positions
-        else:
-            return self
+            enemy_positions.append(self.move(move_part, include_pdn)[1])
+        return self, enemy_positions
 
     def null(self) -> Game:
         """Play a null move."""
         self.move([0, 0])
         return self
 
     def has_player_won(self, player: int = WHITE) -> bool:
@@ -221,64 +215,78 @@
                     if piece.king:
                         black_kings += 1
         if self.variant == 'standard':
             # 25 consecutive non-capture king moves.
             if self.consecutive_noncapture_king_moves >= 50:
                 return True
             # 1 king vs 3 pieces (with at least 1 king) and 16 moves made.
-            if white_pieces == white_kings == 1 and black_pieces == 3 and black_kings >= 1 and self.consecutive_noncapture_king_moves >= 32:
+            if (white_pieces == white_kings == 1 and black_pieces == 3 and black_kings >= 1 and
+                    self.consecutive_noncapture_king_moves >= 32):
                 return True
-            if black_pieces == black_kings == 1 and white_pieces == 3 and white_kings >= 1 and self.consecutive_noncapture_king_moves >= 32:
+            if (black_pieces == black_kings == 1 and white_pieces == 3 and white_kings >= 1 and
+                    self.consecutive_noncapture_king_moves >= 32):
                 return True
             # 1 king vs 2 or fewer pieces (with at least 1 king) and 5 moves made.
-            if white_pieces == white_kings == 1 and black_pieces <= 2 and black_kings >= 1 and self.consecutive_noncapture_king_moves >= 10:
+            if (white_pieces == white_kings == 1 and black_pieces <= 2 and black_kings >= 1 and
+                    self.consecutive_noncapture_king_moves >= 10):
                 return True
-            if black_pieces == black_kings == 1 and white_pieces <= 2 and white_kings >= 1 and self.consecutive_noncapture_king_moves >= 10:
+            if (black_pieces == black_kings == 1 and white_pieces <= 2 and white_kings >= 1 and
+                    self.consecutive_noncapture_king_moves >= 10):
                 return True
             return self.is_threefold()
         elif self.variant in ['frisian', 'frysk!']:
             # 2 kings vs 1 king and 7 moves made.
-            if white_pieces == white_kings == 1 and black_pieces == black_kings == 2 and self.consecutive_noncapture_king_moves >= 14:
+            if (white_pieces == white_kings == 1 and black_pieces == black_kings == 2 and
+                    self.consecutive_noncapture_king_moves >= 14):
                 return True
-            if white_pieces == white_kings == 2 and black_pieces == black_kings == 1 and self.consecutive_noncapture_king_moves >= 14:
+            if (white_pieces == white_kings == 2 and black_pieces == black_kings == 1 and
+                    self.consecutive_noncapture_king_moves >= 14):
                 return True
             # 1 king vs 1 king and 2 moves made (officially immediately if there can't be a forced capture).
             # but we don't detect if there is a forced capture.
             if white_pieces == white_kings == black_pieces == black_kings == 1 and self.consecutive_noncapture_king_moves >= 4:
                 return True
         elif self.variant == 'antidraughts':
             # Only way to draw is threefold.
             return self.is_threefold()
         elif self.variant == 'breakthrough':
             # There is no draw.
             return False
         elif self.variant in ['russian', 'brazilian']:
             # 3 or more kings vs 1 king and 15 moves made.
-            if white_pieces == white_kings == 1 and black_pieces == black_kings >= 3 and self.consecutive_noncapture_king_moves >= 30:
+            if (white_pieces == white_kings == 1 and black_pieces == black_kings >= 3 and
+                    self.consecutive_noncapture_king_moves >= 30):
                 return True
-            if white_pieces == white_kings >= 3 and black_pieces == black_kings == 1 and self.consecutive_noncapture_king_moves >= 30:
+            if (white_pieces == white_kings >= 3 and black_pieces == black_kings == 1 and
+                    self.consecutive_noncapture_king_moves >= 30):
                 return True
             # 15 consecutive non-capture king moves.
             if self.consecutive_noncapture_king_moves >= 30:
                 return True
             # Same number of kings, same number of pieces, 4 or 5 pieces per side and 30 moves made.
-            if white_kings == black_kings >= 1 and white_pieces == black_pieces and white_pieces in [4, 5] and self.moves_since_last_capture >= 60:
+            if (white_kings == black_kings >= 1 and white_pieces == black_pieces and white_pieces in [4, 5] and
+                    self.moves_since_last_capture >= 60):
                 return True
             # Same number of kings, same number of pieces, 6 or 7 pieces per side and 60 moves made.
-            if white_kings == black_kings >= 1 and white_pieces == black_pieces and white_pieces in [6, 7] and self.moves_since_last_capture >= 120:
+            if (white_kings == black_kings >= 1 and white_pieces == black_pieces and white_pieces in [6, 7] and
+                    self.moves_since_last_capture >= 120):
                 return True
             # 3 pieces (with at least 1 king) vs 1 king on the long diagonal and 5 moves made.
-            if white_pieces == 3 and white_kings >= 1 and black_pieces == black_kings == 1 and not white_piece_in_long_diagonal and black_piece_in_long_diagonal and self.moves_since_last_capture >= 10:
+            if (white_pieces == 3 and white_kings >= 1 and black_pieces == black_kings == 1 and
+                    not white_piece_in_long_diagonal and black_piece_in_long_diagonal and self.moves_since_last_capture >= 10):
                 return True
-            if white_pieces == white_kings == 1 and black_pieces == 3 and black_kings >= 1 and white_piece_in_long_diagonal and not black_piece_in_long_diagonal and self.moves_since_last_capture >= 10:
+            if (white_pieces == white_kings == 1 and black_pieces == 3 and black_kings >= 1 and
+                    white_piece_in_long_diagonal and not black_piece_in_long_diagonal and self.moves_since_last_capture >= 10):
                 return True
             # 2 pieces (with at least 1 king) vs 1 king and 5 moves made.
-            if white_pieces == 2 and white_kings >= 1 and black_pieces == black_kings == 1 and self.moves_since_last_capture >= 10:
+            if (white_pieces == 2 and white_kings >= 1 and black_pieces == black_kings == 1 and
+                    self.moves_since_last_capture >= 10):
                 return True
-            if white_pieces == white_kings == 1 and black_pieces == 2 and black_kings >= 1 and self.moves_since_last_capture >= 10:
+            if (white_pieces == white_kings == 1 and black_pieces == 2 and black_kings >= 1 and
+                    self.moves_since_last_capture >= 10):
                 return True
             return self.is_threefold()
         elif self.variant in ['english', 'italian']:
             # 40 non-capture king moves.
             if self.consecutive_noncapture_king_moves >= 80:
                 return True
             return self.is_threefold()
@@ -383,15 +391,15 @@
         turn = self.whose_turn()
         moves = []
         captured_pieces = []
         # get_possible_moves returns only the first jump in a multi-capture sequence,
         # so we use it again after the first jump to check if there are any further moves.
         for move in self.get_possible_moves():
             game_2 = self.copy_fast()
-            _, captures = game_2.move(move, return_captured=True)
+            _, captures = game_2.move(move)
             if game_2.whose_turn() == turn:
                 more_moves, more_captures = game_2.get_moves()
                 for semi_move, semi_capture in zip(more_moves, more_captures):
                     moves.append([move] + semi_move)
                     captured_pieces.append([captures] + semi_capture)
             else:
                 moves.append([move])
@@ -402,15 +410,16 @@
         """Get the legal moves for the current position."""
 
         moves, captures = self.get_moves()
         if not moves:
             return moves, captures
 
         if self.variant in ['frisian', 'frysk!']:
-            # Kings are worth 1.5 and men 1. The kings here are worth 1.501 because if we have a choice between 3 men or 2 kings (both are worth 3) we must capture the kings.
+            # Kings are worth 1.5 and men 1. The kings here are worth 1.501
+            # because if we have a choice between 3 men or 2 kings (both are worth 3) we must capture the kings.
 
             # We have to choose the path that is worth the most.
             king_value = 1.501
             man_value = 1
 
             values = []
             for capture in captures:
@@ -425,21 +434,24 @@
             moves_pseudo_legal = []
             captures_pseudo_legal = []
             for move, capture, value in zip(moves, captures, values):
                 if value == max_value:
                     moves_pseudo_legal.append(move)
                     captures_pseudo_legal.append(capture)
 
-            # If a man and a king can play a capture sequence of equal value, it is forced play the capture sequence with the king.
-            move_with_king = bool(list(filter(lambda move: self.board.searcher.get_piece_by_position(move[0][0]).king, moves_pseudo_legal)))
+            # If a man and a king can play a capture sequence of equal value,
+            # it is forced play the capture sequence with the king.
+            move_with_king = bool(list(filter(lambda move: self.board.searcher.get_piece_by_position(move[0][0]).king,
+                                              moves_pseudo_legal)))
             if move_with_king:
                 moves_pseudo_legal_2 = []
                 captures_pseudo_legal_2 = []
                 for move, capture in zip(moves_pseudo_legal, captures_pseudo_legal):
-                    if self.board.searcher.get_piece_by_position(move[0][0]).king and capture[0] is not None or capture[0] is None:
+                    if (self.board.searcher.get_piece_by_position(move[0][0]).king and capture[0] is not None or
+                            capture[0] is None):
                         moves_pseudo_legal_2.append(move)
                         captures_pseudo_legal_2.append(capture)
             else:
                 moves_pseudo_legal_2 = moves_pseudo_legal
                 captures_pseudo_legal_2 = captures_pseudo_legal
 
             # The same king can't make more than 3 non-capturing moves in a row, if the player has men left.
@@ -447,16 +459,18 @@
             for piece in self.board.searcher.uncaptured_pieces:
                 if piece and not piece.king and piece.player == self.whose_turn():
                     has_man = True
 
             if has_man and len(self.move_stack) >= 6:
                 last_3_move_stack_moves = [self.move_stack[-6], self.move_stack[-4], self.move_stack[-2]]
                 last_3_moves = list(map(lambda move: move.li_one_move, last_3_move_stack_moves))
-                last_3_moves_same_piece = last_3_moves[0][-2:] == last_3_moves[1][:2] and last_3_moves[1][-2:] == last_3_moves[2][:2]
-                was_a_capture = bool(list(filter(bool, [self.capture_stack[-6], self.capture_stack[-4], self.capture_stack[-2]])))
+                last_3_moves_same_piece = (last_3_moves[0][-2:] == last_3_moves[1][:2] and
+                                           last_3_moves[1][-2:] == last_3_moves[2][:2])
+                was_a_capture = bool(list(
+                    filter(bool, [self.capture_stack[-6], self.capture_stack[-4], self.capture_stack[-2]])))
                 loc = int(last_3_moves[-1][-2:])
                 if loc in self.board.searcher.open_positions:
                     is_king = False
                     is_king_for_at_least_3_moves = True
                 else:
                     piece = self.board.searcher.get_piece_by_position(loc)
                     is_king = piece.king
@@ -482,21 +496,24 @@
             moves_pseudo_legal = []
             captures_pseudo_legal = []
             for move, capture in zip(moves, captures):
                 if len(move) == max_len_key:
                     moves_pseudo_legal.append(move)
                     captures_pseudo_legal.append(capture)
 
-            # If a man and a king can play a capture the same number of pieces, it is forced play the capture sequence with the king.
-            move_with_king = bool(list(filter(lambda move: self.board.searcher.get_piece_by_position(move[0][0]).king, moves_pseudo_legal)))
+            # If a man and a king can play a capture the same number of pieces,
+            # it is forced play the capture sequence with the king.
+            move_with_king = bool(list(filter(lambda move: self.board.searcher.get_piece_by_position(
+                move[0][0]).king, moves_pseudo_legal)))
             if move_with_king:
                 moves_pseudo_legal_2 = []
                 captures_pseudo_legal_2 = []
                 for move, capture in zip(moves_pseudo_legal, captures_pseudo_legal):
-                    if self.board.searcher.get_piece_by_position(move[0][0]).king and capture[0] is not None or capture[0] is None:
+                    if self.board.searcher.get_piece_by_position(
+                            move[0][0]).king and capture[0] is not None or capture[0] is None:
                         moves_pseudo_legal_2.append(move)
                         captures_pseudo_legal_2.append(capture)
             else:
                 moves_pseudo_legal_2 = moves_pseudo_legal
                 captures_pseudo_legal_2 = captures_pseudo_legal
 
             # The capture sequence that captures the most kings has to be played.
@@ -553,26 +570,28 @@
             # move_1_captures = [28, 18], move_2_captures = [28, 18, 6]
             # move_2_captures ([28, 18, ...]) starts with the captures in move_1_captures ([28, 18]) and
             # captures more pieces, so move_1 doesn't finish the capture sequence.
             moves_legal = []
             captures_legal = []
             for move, capture in zip(moves, captures):
                 for possible_move, possible_capture in zip(moves, captures):
-                    if move[0][0] == possible_move[0][0] and capture == possible_capture[:len(capture)] and len(possible_capture) > len(capture):
+                    if (move[0][0] == possible_move[0][0] and capture == possible_capture[:len(capture)] and
+                            len(possible_capture) > len(capture)):
                         break
                 else:
                     moves_legal.append(move)
                     captures_legal.append(capture)
 
         elif self.variant == 'english':
             # No restriction. The player can choose, whichever move they prefer.
             # They only have to complete the multi-capture.
             return moves, captures
         else:
-            # Turkish also goes in this category (together with international etc.) because the rule that prohibits a piece from turning 180 degrees is accounted for in get_position_behind_enemy.
+            # Turkish also goes in this category (together with international etc.) because the rule
+            # that prohibits a piece from turning 180 degrees is accounted for in get_position_behind_enemy.
 
             # The move that captures the most pieces has to be played.
             max_len_key = max(list(map(len, moves)))
             moves_legal = []
             captures_legal = []
             for move, capture in zip(moves, captures):
                 if len(move) == max_len_key:
@@ -620,41 +639,45 @@
         for white_piece in white_pieces:
             if '-' in white_piece:
                 start_end = white_piece.split('-')
                 add_for_king = ''
                 if start_end[0][0] == 'K':
                     add_for_king = 'K'
                     start_end[0] = start_end[0][1:]
-                start, end = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square), _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
+                start = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square)
+                end = _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
                 for number in range(start, end + 1):
                     white_pieces_remove_hyphen.append(add_for_king + str(number))
             else:
                 add_for_king = ''
                 if white_piece[0] == 'K':
                     add_for_king = 'K'
                     white_piece = white_piece[1:]
-                white_pieces_remove_hyphen.append(add_for_king + str(_algebraic_to_numeric_square(white_piece, squares_per_letter, every_other_square)))
+                white_pieces_remove_hyphen.append(add_for_king + str(_algebraic_to_numeric_square(
+                    white_piece, squares_per_letter, every_other_square)))
 
         black_pieces_remove_hyphen = []
         for black_piece in black_pieces:
             if '-' in black_piece:
                 start_end = black_piece.split('-')
                 add_for_king = ''
                 if start_end[0][0] == 'K':
                     add_for_king = 'K'
                     start_end[0] = start_end[0][1:]
-                start, end = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square), _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
+                start = _algebraic_to_numeric_square(start_end[0], squares_per_letter, every_other_square)
+                end = _algebraic_to_numeric_square(start_end[1], squares_per_letter, every_other_square)
                 for number in range(start, end + 1):
                     black_pieces_remove_hyphen.append(add_for_king + str(number))
             else:
                 add_for_king = ''
                 if black_piece[0] == 'K':
                     add_for_king = 'K'
                     black_piece = black_piece[1:]
-                black_pieces_remove_hyphen.append(add_for_king + str(_algebraic_to_numeric_square(black_piece, squares_per_letter, every_other_square)))
+                black_pieces_remove_hyphen.append(add_for_king + str(_algebraic_to_numeric_square(
+                    black_piece, squares_per_letter, every_other_square)))
 
         position_count = _get_squares(self.variant)[0]
 
         for index in range(1, position_count + 1):
             str_index = str(index)
             if str_index in white_pieces_remove_hyphen:
                 fen += 'w'
@@ -700,17 +723,19 @@
             row_number = ceil(loc / squares_per_row) - 1  # From get_row_from_position
 
             column = (loc - 1) % squares_per_row  # From get_column
 
             if not half_of_the_squares_are_playable:
                 pass
             elif row_number % 2 == 0:
-                column = (column + 1) * 2 - (2 if bottom_left_square_isnt_playable else 1)  # To account for the always empty white squares
+                # To account for the always empty white squares
+                column = (column + 1) * 2 - (2 if bottom_left_square_isnt_playable else 1)
             else:
-                column = (column + 1) * 2 - (1 if bottom_left_square_isnt_playable else 2)  # To account for the always empty white squares
+                # To account for the always empty white squares
+                column = (column + 1) * 2 - (1 if bottom_left_square_isnt_playable else 2)
 
             piece_symbol = " "
             if loc in self.board.searcher.filled_positions:
                 piece = self.board.searcher.get_piece_by_position(loc)
                 piece_symbol = "w" if piece.player == WHITE else "b"
                 piece_symbol = piece_symbol.upper() if piece.king else piece_symbol
             board[row_number][column] = piece_symbol
```

### Comparing `pydraughts-0.6.3/draughts/core/move.py` & `pydraughts-0.6.4/draughts/core/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 import warnings
 
 warnings.simplefilter("default")
 
 
 class StandardMove:
     """Convert between different move types. Uses internal move representation (white always starts)."""
-    def __init__(self, board: Any = None, board_move: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None, has_captures: Optional[bool] = None, possible_moves: Optional[List[List[List[int]]]] = None, possible_captures: Optional[List[List[Optional[int]]]] = None, hub_to_pdn_pseudolegal: bool = False, variant: Optional[str] = None, is_null: Optional[bool] = None) -> None:
+    def __init__(self, board: Any = None, board_move: Optional[List[List[int]]] = None, hub_move: Optional[str] = None,
+                 hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None,
+                 pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None,
+                 li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None,
+                 has_captures: Optional[bool] = None, possible_moves: Optional[List[List[List[int]]]] = None,
+                 possible_captures: Optional[List[List[Optional[int]]]] = None, hub_to_pdn_pseudolegal: bool = False,
+                 variant: Optional[str] = None, is_null: Optional[bool] = None) -> None:
         self.ambiguous: Optional[bool] = None
         self.captures = None
         self.has_captures = has_captures
         if (possible_moves is None or possible_captures is None) and board:
             self.possible_moves, self.possible_captures = board.legal_moves()
         else:
             self.possible_moves = possible_moves
@@ -20,25 +26,31 @@
         self.variant = variant
         # if not self.variant and board:
         #     self.variant = board.variant
         self.original_pdn_move = pdn_move
         self.is_null = is_null
 
         if self.is_null is None:
-            self.is_null = board_move == [[0, 0]] or hub_move == '0-0' or hub_position_move == '0000' or pdn_move == '0-0' or pdn_position_move == '0000' or steps_move == [0, 0] or li_api_move == ['0000'] or li_one_move == '0000'
+            self.is_null = (board_move == [[0, 0]] or hub_move == '0-0' or hub_position_move == '0000' or
+                            pdn_move == '0-0' or pdn_position_move == '0000' or steps_move == [0, 0] or
+                            li_api_move == ['0000'] or li_one_move == '0000')
 
-        if (board_move or hub_move or hub_position_move or pdn_move or pdn_position_move or steps_move or li_api_move or li_one_move) and not self.is_null:
+        if ((board_move or hub_move or hub_position_move or pdn_move or pdn_position_move or steps_move or li_api_move
+             or li_one_move) and not self.is_null):
             if self.possible_moves:
-                self.board_move = self._to_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self.board_move = self._to_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move,
+                                                 steps_move, li_api_move, li_one_move)
                 self.captures = self.possible_captures[self.possible_moves.index(self.board_move)]
                 self.captures = [] if self.captures[0] is None else self.captures
                 self.has_captures = bool(self.captures)
-                self._from_board(hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self._from_board(hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move,
+                                 li_one_move)
             else:
-                self._no_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self._no_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move,
+                               li_api_move, li_one_move)
         elif self.is_null:
             self.board_move = [[0, 0]]
             self.hub_move = '0-0'
             self.hub_position_move = '0000'
             self.pdn_move = '0-0'
             self.pdn_position_move = '0000'
             self.steps_move = [0, 0]
@@ -59,15 +71,18 @@
         This function exists because hub engines return the captures in alphabetical order
         (e.g. for the move 231201 scan returns 23x01x07x18 instead of 23x01x18x07)
         """
         if captures and captures[0] is None:
             captures = []
         return ''.join(list(sorted(map(self._make_len_2, captures))))
 
-    def _to_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> List[List[int]]:
+    def _to_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None,
+                  hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None,
+                  pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None,
+                  li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> List[List[int]]:
         """Convert the move to a board_move. Requires a Game() object to make the conversions."""
 
         board_move = [] if board_move_given is None else board_move_given
         # Hub related move
 
         if hub_move:
             # Hub move
@@ -89,19 +104,21 @@
 
         # Hub related move
 
         if hub_position_move:
             # Hub position move
 
             # Order the captures
-            hub_position_move_to_use = hub_position_move[:4] + self._sort_captures([int(hub_position_move[i:i + 2]) for i in range(4, len(hub_position_move), 2)])
+            hub_position_move_to_use = hub_position_move[:4] + self._sort_captures(
+                [int(hub_position_move[i:i + 2]) for i in range(4, len(hub_position_move), 2)])
 
             moves_li_board = {}
             for possible_move, possible_capture in zip(self.possible_moves, self.possible_captures):
-                li_move = self._make_len_2(possible_move[0][0]) + self._make_len_2(possible_move[-1][1]) + self._sort_captures(possible_capture)
+                li_move = self._make_len_2(possible_move[0][0]) + self._make_len_2(
+                    possible_move[-1][1]) + self._sort_captures(possible_capture)
                 moves_li_board[li_move] = possible_move
             board_move = moves_li_board[hub_position_move_to_use]
 
         # PDN related move
 
         elif pdn_position_move:
             # PDN position move
@@ -140,15 +157,18 @@
             steps = [int(li_one_move[i:i + 2]) for i in range(0, len(li_one_move), 2)]
             board_move = []
             for index in range(1, len(steps)):
                 board_move.append([steps[index - 1], steps[index]])
 
         return board_move
 
-    def _from_board(self, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> None:
+    def _from_board(self, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None,
+                    pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None,
+                    steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None,
+                    li_one_move: Optional[str] = None) -> None:
         """Convert the move to all other move types. Requires a Game() object to make the conversions."""
 
         hub_move = "" if hub_move is None else hub_move
         hub_position_move = "" if hub_position_move is None else hub_position_move
         pdn_move = "" if pdn_move is None else pdn_move
         pdn_position_move = "" if pdn_position_move is None else pdn_position_move
         steps_move = [] if steps_move is None else steps_move
@@ -257,15 +277,18 @@
         self.hub_position_move = hub_position_move
         self.pdn_move = pdn_move
         self.pdn_position_move = pdn_position_move
         self.steps_move = steps_move
         self.li_api_move = li_api_move
         self.li_one_move = li_one_move
 
-    def _no_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> None:
+    def _no_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None,
+                  hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None,
+                  pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None,
+                  li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> None:
         """Makes as many conversions as possible if the board was not given."""
 
         board_move = [] if board_move_given is None else board_move_given
         hub_move = "" if hub_move is None else hub_move
         hub_position_move = "" if hub_position_move is None else hub_position_move
         pdn_move = "" if pdn_move is None else pdn_move
         pdn_position_move = "" if pdn_position_move is None else pdn_position_move
@@ -293,22 +316,22 @@
             board_move = []
             for index in range(1, len(steps)):
                 board_move.append([steps[index - 1], steps[index]])
 
         if board_move:
             # steps_move
             steps = [board_move[0][0]]
-            for move in board_move:
-                steps.append(move[1])
+            for board_move_part in board_move:
+                steps.append(board_move_part[1])
             steps_move = steps
 
             # li_api_move
             li_api_move = []
-            for move in board_move:
-                move_part = self._make_len_2(move[0]) + self._make_len_2(move[1])
+            for board_move_part in board_move:
+                move_part = self._make_len_2(board_move_part[0]) + self._make_len_2(board_move_part[1])
                 li_api_move.append(move_part)
 
             # li_one_move
             li_one_move = "".join(list(map(self._make_len_2, steps_move)))
 
         # Hub related moves
 
@@ -358,13 +381,7 @@
         self.hub_move = hub_move
         self.hub_position_move = hub_position_move
         self.pdn_move = pdn_move
         self.pdn_position_move = pdn_position_move
         self.steps_move = steps_move
         self.li_api_move = li_api_move
         self.li_one_move = li_one_move
-
-
-class Move(StandardMove):
-    def __init__(self, board: Any = None, board_move: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None, has_captures: Optional[bool] = None, possible_moves: Optional[List[List[List[int]]]] = None, possible_captures: Optional[List[List[Optional[int]]]] = None, hub_to_pdn_pseudolegal: bool = False, variant: Optional[str] = None, is_null: Optional[bool] = None) -> None:
-        warnings.warn("`Move` was renamed to `StandardMove` and a new `Move` was created that doesn't force white to start. Replace `Move` with `StandardMove` in your code. This `Move` will be removed in version 0.7.0.", DeprecationWarning)
-        super().__init__(board, board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move, has_captures, possible_moves, possible_captures, hub_to_pdn_pseudolegal, variant, is_null)
```

### Comparing `pydraughts-0.6.3/draughts/core/piece.py` & `pydraughts-0.6.4/draughts/core/piece.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,17 @@
         if self.possible_capture_moves is None:
             self.possible_capture_moves = self.build_possible_capture_moves(captures)
 
         return self.possible_capture_moves
 
     def build_possible_capture_moves(self, captures: List[int]) -> List[List[int]]:
         """Build all possible capture moves (not positional moves) for this piece."""
-        adjacent_enemy_positions = list(filter((lambda position: position in self.board.searcher.get_positions_by_player(self.other_player)), self.get_adjacent_positions(capture=True)))
+        adjacent_enemy_positions = list(
+            filter((lambda position: position in self.board.searcher.get_positions_by_player(
+                self.other_player)), self.get_adjacent_positions(capture=True)))
         capture_move_positions = []
 
         for enemy_position in adjacent_enemy_positions:
             enemy_piece = self.board.searcher.get_piece_by_position(enemy_position)
 
             if not self.man_can_capture_king and not self.king and enemy_piece.king:
                 continue
@@ -125,15 +127,16 @@
         row_difference = current_row - enemy_row
         column_difference = current_column - enemy_column
 
         # Check if the pieces are on the same row or column
 
         # If half_of_the_squares_are_playable the square in the front is not playable
         # (e.g. a1 is playable but a2 isn't, so the square directly in front of it is a3)
-        if (column_difference == 0 or row_difference == 0) and (row_difference % 2 == 0 if self.half_of_the_squares_are_playable else True):
+        if ((column_difference == 0 or row_difference == 0) and
+                (row_difference % 2 == 0 if self.half_of_the_squares_are_playable else True)):
             next_row = enemy_row - row_difference
             next_column = enemy_column - column_difference
             return [self.get_square(next_row, next_column)]
         return []
 
     def get_diagonal_multiple_squares_behind_enemy(self, enemy_piece: Piece, captures: List[int]) -> List[int]:
         """Get the diagonal squares behind the enemy piece if the piece can move more than one square (kings)."""
@@ -157,17 +160,22 @@
 
         for position in enemy_piece.get_adjacent_positions(capture=True):
             column = (position - 1) % self.board.width
             row = self.get_row_from_position(position)
             down_direction_possible = row > enemy_row
             left_direction_possible = column < enemy_column if enemy_row % 2 == 1 else column <= enemy_column
             # Checks if the captured piece square is between the starting square and the landing square
-            # For example, if the captured piece square is to the left and down of the starting square, we check if the landing square is to the left and down of the captured piece square
-            # It also checks if the position is in a pseudolegal list of legal moves (because we can have landing squares that aren't in the same diagonal as the staring square (e.g. if the piece is in 28, 31 isn't a possible landing square))
-            if down_direction_possible == down_direction and left_direction_possible == left_direction and position in adjacent_positions:
+            # For example, if the captured piece square is to the left and down of the starting square,
+            # we check if the landing square is to the left and down of the captured piece square.
+            #
+            # It also checks if the position is in a pseudolegal list of legal moves
+            # (because we can have landing squares that aren't in the same diagonal as the staring square
+            # (e.g. if the piece is in 28, 31 isn't a possible landing square))
+            if (down_direction_possible == down_direction and left_direction_possible == left_direction and
+                    position in adjacent_positions):
                 legal_adjacent_positions.append(self.get_square(row, column))
 
         enemy_piece.king = was_king
         adjacent_positions = legal_adjacent_positions
 
         positions_to_check = []
         row_to_check = current_row
@@ -246,15 +254,16 @@
         add_column = 0
         if column_difference < 0:
             add_column = -1
         elif column_difference > 0:
             add_column = 1
 
         # Check if the pieces are on the same row or column
-        if (column_difference == 0 or row_difference == 0) and (row_difference % 2 == 0 if self.half_of_the_squares_are_playable else True):
+        if ((column_difference == 0 or row_difference == 0) and (
+                row_difference % 2 == 0 if self.half_of_the_squares_are_playable else True)):
             for multiplier in range(1, max(self.board.width, self.board.height)):
                 # In frisian, the square directly in front, behind, on the left and on the right of the piece
                 # isn't playable. We only skip if 'column_difference == 0' because the squares on the right and left,
                 # even though they have a distance of two squares (including non-playable squares),
                 # it is considered as the next column.
                 if multiplier % 2 == 1 and self.half_of_the_squares_are_playable and column_difference == 0:
                     continue
@@ -345,15 +354,16 @@
         """Create moves ([[cur_pos, end_pos1], [cur_pos, end_pos2]]) given the ending square ([end_pos1, end_pos2])."""
         return [[self.position, new_position] for new_position in new_positions]
 
     def get_adjacent_positions(self, capture: bool = False) -> List[int]:
         """Get all adjacent positions of the piece."""
         # In some variants men can't capture backwards
         criteria = bool(capture or self.king) if self.men_can_capture_backwards else bool(self.king)
-        return self.get_directional_adjacent_positions(forward=True, capture=capture) + (self.get_directional_adjacent_positions(forward=False, capture=capture) if criteria else [])
+        return self.get_directional_adjacent_positions(forward=True, capture=capture) + (
+            self.get_directional_adjacent_positions(forward=False, capture=capture) if criteria else [])
 
     def get_column(self) -> int:
         """Get the piece's column."""
         width: int = self.board.width
         return (self.position - 1) % width
 
     def get_row(self) -> int:
@@ -473,15 +483,16 @@
             return []
         positions = []
         current_row = self.get_row()
         current_column = self.get_column()
         row_in_front = 2 if self.half_of_the_squares_are_playable else 1
 
         for multiplier in range(1, self.board.height):
-            next_row = current_row + multiplier * (row_in_front if self.player == BLACK else -row_in_front) * (1 if forward else -1)
+            next_row = current_row + multiplier * (row_in_front if self.player == BLACK else -row_in_front) * (
+                1 if forward else -1)
             if next_row in self.board.position_layout:
                 positions.append(self.board.position_layout[next_row][current_column])
 
         for multiplier in range(1, self.board.width):
             next_column = current_column + multiplier * (1 if self.player == BLACK else -1) * (1 if forward else -1)
             if next_column in self.board.position_layout[current_row]:
                 positions.append(self.board.position_layout[current_row][next_column])
@@ -505,15 +516,16 @@
             else:
                 if self.diagonal_moves:
                     positions += self.get_directional_diagonal_one_square_adjacent_positions(forward)
                 if self.orthogonal_captures:
                     positions += self.get_directional_orthogonal_one_square_adjacent_positions(forward, capture)
         return positions
 
-    def get_next_column_indexes(self, current_row: int, current_column: int, i: int = 1, unfiltered: bool = False) -> List[int]:
+    def get_next_column_indexes(self, current_row: int, current_column: int, i: int = 1, unfiltered: bool = False
+                                ) -> List[int]:
         """
         Get the index of the next column.
         It isn't as simple as finding the next row (where we only add or subtract 1) but the column index only changes
         once every 2 rows.
         e.g. Square 32 and 27 are both in the second row, but 27 and 31 are not.
         :param i: current_row ± i is the row we should search (the columns for current_row + i are the same as current_row - i).
         e.g. if current row=3 and i=2, we will return the 2 possible columns for row 5 (which will be the same for row 1).
```

### Comparing `pydraughts-0.6.3/draughts/core/variant.py` & `pydraughts-0.6.4/draughts/core/variant.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from __future__ import annotations
 from draughts.core.game import Game, _convert_variant_names
-from draughts.convert import fen_from_variant, fen_to_variant, move_from_variant, move_to_variant, _number_to_algebraic, _algebraic_to_number
+from draughts.convert import (fen_from_variant, fen_to_variant, move_from_variant, move_to_variant,
+                              _number_to_algebraic, _algebraic_to_number)
 from draughts.core.move import StandardMove
 import pickle
 from typing import Optional, Any, List, Tuple
 
 WHITE = 2
 BLACK = 1
 
 
 class Move(StandardMove):
     """Convert between different move types. Accounts for the differences between variants."""
-    def __init__(self, board: Any = None, board_move: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None, has_captures: Optional[bool] = None, possible_moves: Optional[List[List[List[int]]]] = None, possible_captures: Optional[List[List[Optional[int]]]] = None, hub_to_pdn_pseudolegal: bool = False, variant: Optional[str] = None, is_null: Optional[bool] = None) -> None:
+    def __init__(self, board: Any = None, board_move: Optional[List[List[int]]] = None, hub_move: Optional[str] = None,
+                 hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None,
+                 pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None,
+                 li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None,
+                 has_captures: Optional[bool] = None, possible_moves: Optional[List[List[List[int]]]] = None,
+                 possible_captures: Optional[List[List[Optional[int]]]] = None, hub_to_pdn_pseudolegal: bool = False,
+                 variant: Optional[str] = None, is_null: Optional[bool] = None) -> None:
         self.ambiguous: Optional[bool] = None
         self.captures = None
         self.to_algebraic_variant = None
         self.has_captures = has_captures
         if (possible_moves is None or possible_captures is None) and board:
             self.possible_moves, self.possible_captures = board._legal_moves_board()
         else:
@@ -27,36 +34,45 @@
         self.variant = variant
         if not self.variant and board:
             self.variant = board.variant
         self.original_pdn_move = pdn_move
         self.is_null = is_null
 
         if self.is_null is None:
-            self.is_null = board_move == [[0, 0]] or hub_move == '0-0' or hub_position_move == '0000' or pdn_move == '0-0' or pdn_position_move == '0000' or steps_move == [0, 0] or li_api_move == ['0000'] or li_one_move == '0000'
+            self.is_null = (board_move == [[0, 0]] or hub_move == '0-0' or hub_position_move == '0000' or
+                            pdn_move == '0-0' or pdn_position_move == '0000' or steps_move == [0, 0] or
+                            li_api_move == ['0000'] or li_one_move == '0000')
 
-        if (board_move or hub_move or hub_position_move or pdn_move or pdn_position_move or steps_move or li_api_move or li_one_move) and not self.is_null:
+        if ((board_move or hub_move or hub_position_move or pdn_move or pdn_position_move or steps_move or
+             li_api_move or li_one_move) and not self.is_null):
             if self.possible_moves:
-                self.board_move = self._to_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self.board_move = self._to_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move,
+                                                 steps_move, li_api_move, li_one_move)
                 self.captures = self.possible_captures[self.possible_moves.index(self.board_move)]
                 self.captures = [] if self.captures[0] is None else self.captures
                 self.has_captures = bool(self.captures)
-                self._from_board(hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self._from_board(hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move,
+                                 li_one_move)
             else:
-                self._no_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move, li_api_move, li_one_move)
+                self._no_board(board_move, hub_move, hub_position_move, pdn_move, pdn_position_move, steps_move,
+                               li_api_move, li_one_move)
         elif self.is_null:
             self.board_move = [[0, 0]]
             self.hub_move = '0-0'
             self.hub_position_move = '0000'
             self.pdn_move = '0-0'
             self.pdn_position_move = '0000'
             self.steps_move = [0, 0]
             self.li_api_move = ['0000']
             self.li_one_move = '0000'
 
-    def _to_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> List[List[int]]:
+    def _to_board(self, board_move_given: Optional[List[List[int]]] = None, hub_move: Optional[str] = None,
+                  hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None,
+                  pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None,
+                  li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> List[List[int]]:
         """Convert the move to a board_move. Requires a Board() object to make the conversions."""
 
         board_move = [] if board_move_given is None else board_move_given
         # Hub related move
 
         if hub_move:
             # Hub move
@@ -78,19 +94,21 @@
 
         # Hub related move
 
         if hub_position_move:
             # Hub position move
 
             # Order the captures
-            hub_position_move_to_use = hub_position_move[:4] + self._sort_captures([int(hub_position_move[i:i + 2]) for i in range(4, len(hub_position_move), 2)])
+            hub_position_move_to_use = hub_position_move[:4] + self._sort_captures(
+                [int(hub_position_move[i:i + 2]) for i in range(4, len(hub_position_move), 2)])
 
             moves_li_board = {}
             for possible_move, possible_capture in zip(self.possible_moves, self.possible_captures):
-                li_move = self._make_len_2(possible_move[0][0]) + self._make_len_2(possible_move[-1][1]) + self._sort_captures(possible_capture)
+                li_move = self._make_len_2(possible_move[0][0]) + self._make_len_2(
+                    possible_move[-1][1]) + self._sort_captures(possible_capture)
                 moves_li_board[li_move] = possible_move
             board_move = moves_li_board[hub_position_move_to_use]
 
         # PDN related move
 
         elif pdn_position_move:
             # PDN position move
@@ -129,15 +147,18 @@
             steps = [int(li_one_move[i:i + 2]) for i in range(0, len(li_one_move), 2)]
             board_move = []
             for index in range(1, len(steps)):
                 board_move.append([steps[index - 1], steps[index]])
 
         return board_move
 
-    def _from_board(self, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None, pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None, steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None, li_one_move: Optional[str] = None) -> None:
+    def _from_board(self, hub_move: Optional[str] = None, hub_position_move: Optional[str] = None,
+                    pdn_move: Optional[str] = None, pdn_position_move: Optional[str] = None,
+                    steps_move: Optional[List[int]] = None, li_api_move: Optional[List[str]] = None,
+                    li_one_move: Optional[str] = None) -> None:
         """Convert the move to all other move types. Requires a Board() object to make the conversions."""
 
         hub_move = "" if hub_move is None else hub_move
         hub_position_move = "" if hub_position_move is None else hub_position_move
         pdn_move = "" if pdn_move is None else pdn_move
         pdn_position_move = "" if pdn_position_move is None else pdn_position_move
         steps_move = [] if steps_move is None else steps_move
@@ -255,29 +276,36 @@
 
 class Board:
     """A draughts game which considers the variant."""
     def __init__(self, variant: str = "standard", fen: str = "startpos"):
         self.variant = _convert_variant_names(variant)
         self._game = Game(variant, fen_from_variant(fen, variant) if fen != "startpos" else fen)
         self.initial_fen = fen_to_variant(self._game.initial_fen, self.variant)
-        self.move_stack = []
+        self.move_stack: List[Move] = []
         self.fens = [self.initial_fen]
 
         self._last_non_reversible_fen = self.initial_fen
-        self._reversible_moves = []
+        self._last_non_reversible_fens: List[str] = [self._last_non_reversible_fen]
+        self._reversible_moves: List[Move] = []
 
     def copy(self) -> Board:
         """Copy the board (transfers all data)."""
         # At least 6 times faster than deepcopy.
-        return pickle.loads(pickle.dumps(self, -1))
+        new_board: Board = pickle.loads(pickle.dumps(self, -1))
+        return new_board
 
     def pop(self) -> Board:
         """Undo the last move."""
         self._game.pop()
         self.fens.pop()
+        self.move_stack.pop()
+        self._last_non_reversible_fens.pop()
+        self._last_non_reversible_fen = self._last_non_reversible_fens[-1]
+        if self._reversible_moves:
+            self._reversible_moves.pop()
         return self
 
     def push(self, move: Move) -> Board:
         """Make a move."""
         self.move_stack.append(move)
         board_move = move.board_move.copy()
         for index, steps in enumerate(board_move):
@@ -285,14 +313,15 @@
         self._game.push(board_move)
         self.fens.append(fen_to_variant(self._game.get_li_fen(), self.variant))
         if self._game.reversible_moves:
             self._reversible_moves.append(move)
         else:
             self._reversible_moves = []
             self._last_non_reversible_fen = self.fen
+        self._last_non_reversible_fens.append(self._last_non_reversible_fen)
         return self
 
     def null(self) -> Board:
         """Play a null move."""
         self.push(Move(self, steps_move=[0, 0]))
         self.fens.append(fen_to_variant(self._game.get_li_fen(), self.variant))
         return self
@@ -315,22 +344,25 @@
         return self.fens[-1]
 
     def _legal_moves_board(self) -> Tuple[List[List[List[int]]], List[List[Optional[int]]]]:
         """Get the legal moves for the current position in board_move format."""
         legal_moves, legal_captures = self._game.legal_moves()
         for move_index, move_capture in enumerate(zip(legal_moves, legal_captures)):
             for index, steps in enumerate(move_capture[0]):
-                legal_moves[move_index][index] = list(map(lambda square: int(move_to_variant(str(square), variant=self.variant, to_algebraic=False)), steps))
-            legal_captures[move_index] = list(map(lambda square: None if square is None else int(move_to_variant(str(square), variant=self.variant, to_algebraic=False)), move_capture[1]))
+                legal_moves[move_index][index] = list(map(lambda square: int(move_to_variant(
+                    str(square), variant=self.variant, to_algebraic=False)), steps))
+            legal_captures[move_index] = list(map(lambda square: None if square is None else int(move_to_variant(
+                str(square), variant=self.variant, to_algebraic=False)), move_capture[1]))
         return legal_moves, legal_captures
 
     def legal_moves(self) -> List[Move]:
         """Get the legal moves for the current position."""
-        legal_moves, legal_captures = self._legal_moves_board()
-        legal_moves = list(map(lambda move: Move(board_move=move, possible_moves=legal_moves, possible_captures=legal_captures), legal_moves))
+        legal_board_moves, legal_captures = self._legal_moves_board()
+        legal_moves: List[Move] = list(map(lambda board_move: Move(
+            board_move=board_move, possible_moves=legal_board_moves, possible_captures=legal_captures), legal_board_moves))
         return legal_moves
 
     @property
     def turn(self) -> int:
         """Get whose turn it is."""
         game_turn = self._game.whose_turn()
         return 3 - game_turn if self.variant == "english" else game_turn
```

### Comparing `pydraughts-0.6.3/draughts/engine.py` & `pydraughts-0.6.4/draughts/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from draughts.engines.checkerboard import CheckerBoardEngine
 from typing import Optional, Union, Dict, Any
 from draughts.core.variant import Move
 
 
 class Limit:
     """Conditions on when the engine should stop searching."""
-    def __init__(self, time: Union[int, float, None] = None, inc: Union[int, float, None] = None, depth: Optional[int] = None, nodes: Optional[int] = None, movetime: Union[int, float, None] = None):
+    def __init__(self, time: Union[int, float, None] = None, inc: Union[int, float, None] = None,
+                 depth: Optional[int] = None, nodes: Optional[int] = None, movetime: Union[int, float, None] = None):
         assert time is not None or depth is not None or nodes is not None or movetime is not None
         self.time = time
         self.inc = inc
         self.depth = depth
         self.nodes = nodes
         self.movetime = movetime
 
 
 class PlayResult:
     """The outcome of the engine search."""
-    def __init__(self, move: Optional[Move] = None, ponder: Optional[Move] = None, info: Optional[Dict[str, Any]] = None, draw_offered: bool = False, resigned: bool = False):
+    def __init__(self, move: Optional[Move] = None, ponder: Optional[Move] = None, info: Optional[Dict[str, Any]] = None,
+                 draw_offered: bool = False, resigned: bool = False):
         self.move = move
         self.ponder = ponder
         self.info = info
         self.draw_offered = draw_offered
         self.resigned = resigned
```

### Comparing `pydraughts-0.6.3/draughts/engines/checkerboard.py` & `pydraughts-0.6.4/draughts/engines/checkerboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,45 +7,47 @@
 from draughts.convert import move_to_variant
 from typing import Union, List, Any, Dict, Tuple
 
 logger = logging.getLogger("pydraughts")
 
 
 class CheckerBoardEngine:
-    def __init__(self, command: Union[List[str], str], divide_time_by: int = 40, checkerboard_timing: bool = False, ENGINE: int = 5) -> None:
+    def __init__(self, command: Union[List[str], str], divide_time_by: int = 40, checkerboard_timing: bool = False,
+                 ENGINE: int = 5) -> None:
         if type(command) == str:
             command = [command]
         command = list(filter(bool, command))
         command = " ".join(command)
         if "\\" not in command and "/" not in command:
             self.cwd = os.path.realpath(os.path.expanduser("."))
             self.command = os.path.join(self.cwd, command)
         else:
             self.command = command
         self.ENGINE = ENGINE
-        self.info = None
+        self.info = ""
         self.id = {}
         self.result = None
         self.divide_time_by = divide_time_by
         self.checkerboard_timing = checkerboard_timing
         self._sent_variant = False
+        self.engine: Union[Engine64, Engine32]
         self.engine, self.bits = self._open_engine()
         self.id["name"] = self.engine.enginecommand('name')[0].decode()
 
     def _open_engine(self) -> Union[Tuple[Engine64, int], Tuple[Engine32, int]]:
         """Open the engine process."""
         try:
             return Engine64(self.command), 64
         except Exception:
             return Engine32(self.command), 32
 
     def setoption(self, name: str, value: Union[str, int]) -> None:
         """Set an engine option."""
         if name == 'divide-time-by':
-            self.divide_time_by = value
+            self.divide_time_by = int(value)
         else:
             self.engine.enginecommand(f"set {name} {value}")
 
     def configure(self, options: Dict[str, Union[str, int]]) -> None:
         """Configure many options at once."""
         for name, value in options.items():
             self.setoption(name, value)
@@ -76,15 +78,16 @@
             elif board.variant == 'italian':
                 self.engine.enginecommand('set gametype 22')
             elif board.variant == 'english':
                 self.engine.enginecommand('set gametype 21')
             self._sent_variant = True
 
         if board.move_stack:
-            gamehist = f'set gamehist {board._last_non_reversible_fen} {" ".join(list(map(lambda move: move.pdn_move, board._reversible_moves)))}'
+            reversible_moves = " ".join(list(map(lambda move: move.pdn_move, board._reversible_moves)))
+            gamehist = f'set gamehist {board._last_non_reversible_fen} {reversible_moves}'
             if len(gamehist) > 256:
                 gamehist = " ".join(gamehist[-256:].split()[1:])
             self.engine.enginecommand(gamehist)
 
         time_to_use = None
         if time:
 
@@ -108,48 +111,50 @@
             else:
                 time_to_use = time / self.divide_time_by
 
         logger.debug(f"Fen: {board.fen}, Time to use: {time_to_use}, Time: {time}, Inc: {inc}, Movetime: {movetime}")
 
         hub_pos_move, info, cbmove, result = self.engine.getmove(board, time_to_use, time, inc, movetime)
 
-        logger.debug(f"Hub Pos Move: {hub_pos_move}, CBMove: {cbmove}, Info: {info}, Result: {result}")
+        logger.debug(f"Hub Pos Move: {hub_pos_move}, CBMove: {cbmove}, Info: {info.decode()}, Result: {result}")
 
         if hub_pos_move:
             hub_move = '-'.join([hub_pos_move[i:i+2] for i in range(0, len(hub_pos_move), 2)])
             bestmove = draughts.Move(board, hub_move=move_to_variant(hub_move, board.variant, to_algebraic=False))
         else:
             steps = []
             positions = [cbmove['from']]
             jumps = max(cbmove['jumps'], 1)
             for pos in cbmove['path'][1:jumps]:
                 positions.append(pos)
             positions.append(cbmove['to'])
             for pos in positions:
-                steps.append(self._row_col_to_num(board, pos[1], pos[0]))  # Checkerboard returns first the column, then the row
+                # Checkerboard returns first the column, then the row
+                steps.append(self._row_col_to_num(board, pos[1], pos[0]))
 
             steps = list(map(lambda step: int(move_to_variant(str(step), board.variant, to_algebraic=False)), steps))
             bestmove = draughts.Move(board, steps_move=steps)
 
         self.info = info.decode()
         self.result = result
         return draughts.engine.PlayResult(bestmove, None, {'info': self.info, 'result': self.result})
 
     def _row_col_to_num(self, board: draughts.Board, row: int, col: int) -> int:
         """Get the square from the row and column."""
         if row % 2 == 0:
-            col = ((col + 2) / 2) - 1
+            col = int(((col + 2) / 2) - 1)
         else:
-            col = ((col + 1) / 2) - 1
+            col = int(((col + 1) / 2) - 1)
         # Because:
         # 1. In italian the bottom-left square isn't playable, so in CheckerBoard the board is flipped vertically.
         # 2. In most variants the bottom-left square for the starting side (usually white) is in column a,
         # while in english black starts, so the bottom-left square for the starting side (black) is in row h.
         flip_column = board.variant not in ['english', 'italian']
         if flip_column:
             col = board._game.board.width - 1 - col
         # Because in english black starts
         white_starts = board.variant not in ['english']
         if not white_starts:
             row = (board._game.board.height - 1) - row
         loc = board._game.board.position_layout.get(row, {}).get(col)
+        assert isinstance(loc, int)
         return loc
```

### Comparing `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_64.py` & `pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
     def enginecommand(self, command: str) -> Tuple[bytes, int]:
         """Send an enginecommand to the engine."""
         output = ctypes.create_string_buffer(b'', 1024)
         result = self.engine.enginecommand(ctypes.create_string_buffer(bytes(command.encode('ascii')), 256), output)
         return output.value, result
 
-    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None, increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
+    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None,
+                increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None
+                ) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
         """Send a getmove to the engine."""
         assert maxtime is not None or time is not None or movetime is not None
 
         # From CheckerBoard API:
         WHITE = 1
         BLACK = 2
 
@@ -41,15 +43,15 @@
         # Reversed color because red (black) starts first and not white in english checkers in Checkerboard.
         color = WHITE if game.turn == draughts.WHITE else BLACK
 
         info = 0
         moreinfo = 0
         if movetime:
             info = info | (1 << 1)  # 2nd bit means the engine has to think for exactly maxtime seconds
-        elif time:
+        elif time is not None and increment is not None:
             if time / .01 > 2 ** 15 - 1 or increment / .01 > 2 ** 15 - 1:
                 info = info | (1 << 3)  # 0.1 seconds
                 info = info | (1 << 4)  # 0.1 seconds
                 time = int(time / .1)
                 increment = int(increment / .1)
             elif time / .001 > 2 ** 15 - 1 or increment / .001 > 2 ** 15 - 1:
                 info = info | (1 << 3)  # 0.01 seconds
@@ -63,32 +65,36 @@
             if len(bin_time) > 16:
                 bin_time = '1' * 16
             bin_inc = bin(increment)[2:].zfill(16)
             if len(bin_inc) > 16:
                 bin_inc = '1' * 16
             moreinfo = eval('0b' + bin_time + bin_inc)
 
-        if movetime:
-            maxtime = ctypes.c_double(float(movetime))
+        if movetime is not None:
+            maxtime_double = ctypes.c_double(float(movetime))
         else:
-            maxtime = ctypes.c_double(float(maxtime))
+            assert maxtime is not None
+            maxtime_double = ctypes.c_double(float(maxtime))
         output = ctypes.create_string_buffer(b'', 1024)
         playnow = ctypes.c_int(0)
 
         class coor(ctypes.Structure):
             _fields_ = [("x", ctypes.c_int), ("y", ctypes.c_int)]
 
         class CBmove(ctypes.Structure):
-            _fields_ = [("jumps", ctypes.c_int), ("newpiece", ctypes.c_int), ("oldpiece", ctypes.c_int), ("from", coor), ("to", coor), ("path", coor * 12), ("del", coor * 12), ("delpiece", ctypes.c_int * 12)]
+            _fields_ = [("jumps", ctypes.c_int), ("newpiece", ctypes.c_int), ("oldpiece", ctypes.c_int), ("from", coor),
+                        ("to", coor), ("path", coor * 12), ("del", coor * 12), ("delpiece", ctypes.c_int * 12)]
 
-        self.engine.argtypes = [((ctypes.c_int * 8) * 8), ctypes.c_int, ctypes.c_double, (ctypes.c_char * 1024), ctypes.POINTER(ctypes.c_int), ctypes.c_int, ctypes.c_int, ctypes.POINTER(CBmove)]
+        # self.engine.argtypes = [((ctypes.c_int * 8) * 8), ctypes.c_int, ctypes.c_double, (ctypes.c_char * 1024),
+        #                         ctypes.POINTER(ctypes.c_int), ctypes.c_int, ctypes.c_int, ctypes.POINTER(CBmove)]
 
         cbmove = CBmove()
 
-        result = self.engine.getmove(board, color, maxtime, output, ctypes.byref(playnow), info, moreinfo,  ctypes.byref(cbmove))
+        result = self.engine.getmove(board, color, maxtime_double, output, ctypes.byref(playnow), info, moreinfo,
+                                     ctypes.byref(cbmove))
 
         old_fen = game._game.get_fen()
         new_fen = from_board(board, game)
         our_pieces, opponents_pieces = (['w', 'W'], ['b', 'B']) if old_fen[0] == 'W' else (['b', 'B'], ['w', 'W'])
         captures = []
         start_pos, end_pos = None, None
         for index in range(1, len(old_fen)):
@@ -96,15 +102,16 @@
                 start_pos = index
             elif new_fen[index] in our_pieces and old_fen[index] == 'e':
                 end_pos = index
             elif old_fen[index] in opponents_pieces and new_fen[index] == 'e':
                 captures.append(index)
         hub_pos_move = None
         if start_pos and end_pos:
-            hub_pos_move = game._game.make_len_2(start_pos) + game._game.make_len_2(end_pos) + game._game.sort_captures(captures)
+            hub_pos_move = game._game.make_len_2(start_pos) + game._game.make_len_2(end_pos) + game._game.sort_captures(
+                captures)
 
         cbmove_output_2 = {}
         cbmove_output_2['jumps'] = cbmove.jumps
         cbmove_output_2['oldpiece'] = cbmove.oldpiece
         cbmove_output_2['newpiece'] = cbmove.newpiece
         cbmove_output_2['to'] = cbmove.to.x, cbmove.to.y
         cbmove.to = getattr(cbmove, 'from')
```

### Comparing `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_client.py` & `pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 
 class Engine32(Client64):
     """64 bit client to communicate with the 32 bit server that is running the old Checkerboard engine."""
     def __init__(self, command: str) -> None:
 
         command = command.replace('\\', '\\\\')
 
-        super(Engine32, self).__init__(module32='engine_server', append_sys_path=os.path.dirname(__file__), dll_name=command)
+        super(Engine32, self).__init__(module32='engine_server', append_sys_path=os.path.dirname(__file__), timeout=15.,
+                                       dll_name=command)
 
     def enginecommand(self, command: str) -> Tuple[bytes, int]:
         """Send an enginecommand to the engine."""
-        return self.request32('enginecommand', command)
+        response: Tuple[bytes, int] = self.request32('enginecommand', command)
+        return response
 
-    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None, increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
+    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None,
+                increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None
+                ) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
         """Send a getmove to the engine."""
         assert maxtime is not None or time is not None or movetime is not None
-        return self.request32('getmove', game, maxtime, time, increment, movetime)
+        response: Tuple[Optional[str], bytes, Dict[str, Any], int] = self.request32('getmove', game, maxtime, time,
+                                                                                    increment, movetime)
+        return response
```

### Comparing `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_server.py` & `pydraughts-0.6.4/draughts/engines/checkerboard_extra/engine_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import ctypes
 import draughts
 from draughts.engines.checkerboard_extra.get_checker_board import get_board, from_board
-import os
 from typing import Tuple, Optional, Union, Dict, Any
 
 from msl.loadlib import Server32
 
 
 class Engine32Server(Server32):
     """32 bit server to run old Checkerboard engines."""
@@ -15,15 +14,17 @@
 
     def enginecommand(self, command: str) -> Tuple[bytes, int]:
         """Send an enginecommand to the engine."""
         output = ctypes.create_string_buffer(b'', 1024)
         result = self.lib.enginecommand(ctypes.create_string_buffer(bytes(command.encode('ascii')), 256), output)
         return output.value, result
 
-    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None, increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
+    def getmove(self, game: draughts.Board, maxtime: Union[int, float, None] = None, time: Union[int, float, None] = None,
+                increment: Union[int, float, None] = None, movetime: Union[int, float, None] = None
+                ) -> Tuple[Optional[str], bytes, Dict[str, Any], int]:
         """Send a getmove to the engine."""
 
         # From CheckerBoard API:
         WHITE = 1
         BLACK = 2
 
         board = get_board(game)
@@ -31,15 +32,15 @@
         # Reversed color because red (black) starts first and not white in english checkers in Checkerboard.
         color = WHITE if game.turn == draughts.WHITE else BLACK
 
         info = 0
         moreinfo = 0
         if movetime:
             info = info | (1 << 1)  # 2nd bit means the engine has to think for exactly maxtime seconds
-        elif time:
+        elif time is not None and increment is not None:
             if time / .01 > 2 ** 15 - 1 or increment / .01 > 2 ** 15 - 1:
                 info = info | (1 << 3)  # 0.1 seconds
                 info = info | (1 << 4)  # 0.1 seconds
                 time = int(time / .1)
                 increment = int(increment / .1)
             elif time / .001 > 2 ** 15 - 1 or increment / .001 > 2 ** 15 - 1:
                 info = info | (1 << 3)  # 0.01 seconds
@@ -53,32 +54,36 @@
             if len(bin_time) > 16:
                 bin_time = '1' * 16
             bin_inc = bin(increment)[2:].zfill(16)
             if len(bin_inc) > 16:
                 bin_inc = '1' * 16
             moreinfo = eval('0b' + bin_time + bin_inc)
 
-        if movetime:
-            maxtime = ctypes.c_double(float(movetime))
+        if movetime is not None:
+            maxtime_double = ctypes.c_double(float(movetime))
         else:
-            maxtime = ctypes.c_double(float(maxtime))
+            assert maxtime is not None
+            maxtime_double = ctypes.c_double(float(maxtime))
         output = ctypes.create_string_buffer(b'', 1024)
         playnow = ctypes.c_int(0)
 
         class coor(ctypes.Structure):
             _fields_ = [("x", ctypes.c_int), ("y", ctypes.c_int)]
 
         class CBmove(ctypes.Structure):
-            _fields_ = [("jumps", ctypes.c_int), ("newpiece", ctypes.c_int), ("oldpiece", ctypes.c_int), ("from", coor), ("to", coor), ("path", coor * 12), ("del", coor * 12), ("delpiece", ctypes.c_int * 12)]
+            _fields_ = [("jumps", ctypes.c_int), ("newpiece", ctypes.c_int), ("oldpiece", ctypes.c_int), ("from", coor),
+                        ("to", coor), ("path", coor * 12), ("del", coor * 12), ("delpiece", ctypes.c_int * 12)]
 
-        self.lib.getmove.argtypes = [((ctypes.c_int * 8) * 8), ctypes.c_int, ctypes.c_double, (ctypes.c_char * 1024), ctypes.POINTER(ctypes.c_int), ctypes.c_int, ctypes.c_int, ctypes.POINTER(CBmove)]
+        # self.lib.getmove.argtypes = [((ctypes.c_int * 8) * 8), ctypes.c_int, ctypes.c_double, (ctypes.c_char * 1024),
+        #                              ctypes.POINTER(ctypes.c_int), ctypes.c_int, ctypes.c_int, ctypes.POINTER(CBmove)]
 
         cbmove = CBmove()
 
-        result = self.lib.getmove(board, color, maxtime, output, ctypes.byref(playnow), info, moreinfo, ctypes.byref(cbmove))
+        result = self.lib.getmove(board, color, maxtime_double, output, ctypes.byref(playnow), info, moreinfo,
+                                  ctypes.byref(cbmove))
 
         old_fen = game._game.get_fen()
         new_fen = from_board(board, game)
         our_pieces, opponents_pieces = (['w', 'W'], ['b', 'B']) if old_fen[0] == 'W' else (['b', 'B'], ['w', 'W'])
         captures = []
         start_pos, end_pos = None, None
         for index in range(1, len(old_fen)):
@@ -86,15 +91,16 @@
                 start_pos = index
             elif new_fen[index] in our_pieces and old_fen[index] == 'e':
                 end_pos = index
             elif old_fen[index] in opponents_pieces and new_fen[index] == 'e':
                 captures.append(index)
         hub_pos_move = None
         if start_pos and end_pos:
-            hub_pos_move = game._game.make_len_2(start_pos) + game._game.make_len_2(end_pos) + game._game.sort_captures(captures)
+            hub_pos_move = game._game.make_len_2(start_pos) + game._game.make_len_2(end_pos) + game._game.sort_captures(
+                captures)
 
         cbmove_output_2 = {}
         cbmove_output_2['jumps'] = cbmove.jumps
         cbmove_output_2['oldpiece'] = cbmove.oldpiece
         cbmove_output_2['newpiece'] = cbmove.newpiece
         cbmove_output_2['to'] = cbmove.to.x, cbmove.to.y
         cbmove.to = getattr(cbmove, 'from')
```

### Comparing `pydraughts-0.6.3/draughts/engines/checkerboard_extra/get_checker_board.py` & `pydraughts-0.6.4/draughts/engines/checkerboard_extra/get_checker_board.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/draughts/engines/dxp.py` & `pydraughts-0.6.4/draughts/engines/dxp.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import draughts.engine
 import subprocess
 import os
 import signal
 import threading
 import time
 import logging
-from typing import Optional, Dict, Union, List, Any
+from typing import Optional, Dict, Union, List, Any, Tuple
 
 logger = logging.getLogger("pydraughts")
 
 
 class DXPEngine:
-    def __init__(self, command: Union[List[str], str, None] = None, options: Optional[Dict[str, Union[str, int, bool]]] = None, initial_time: int = 0, cwd: Optional[str] = None, ENGINE: int = 5) -> None:
+    def __init__(self, command: Union[List[str], str, None] = None,
+                 options: Optional[Dict[str, Union[str, int, bool]]] = None, initial_time: int = 0,
+                 cwd: Optional[str] = None, ENGINE: int = 5) -> None:
         if options is None:
             options = {}
         self.initial_time = initial_time
         self.max_moves = 0
         self.ip = '127.0.0.1'
         self.port = '27531'
         self.command = command
@@ -34,47 +36,48 @@
         self.configure(options)
 
         if not self.engine_opened:
             cwd = cwd or os.getcwd()
             cwd = os.path.realpath(os.path.expanduser(cwd))
             if type(command) == str:
                 command = [command]
-            command = list(filter(bool, command))
+            command = list(filter(None, command))
             command[0] = os.path.realpath(os.path.expanduser(command[0]))
             command[0] = '"' + command[0] + '"'
             command = ' '.join(command)
             self.command = command
             self.p = self._open_process(command, cwd)
             self.engine_receive_thread = threading.Thread(target=self._recv)
             self.engine_receive_thread.start()
 
         self.start_time = time.perf_counter_ns()
         self.quit_time = 0
 
     def setoption(self, name: str, value: Union[str, int, bool]) -> None:
         """Set a DXP option."""
         if name == 'engine-opened':
-            self.engine_opened = value
+            self.engine_opened = bool(value)
         elif name == 'ip':
             self.ip = str(value)
         elif name == 'port':
             self.port = str(value)
         elif name == 'wait-to-open-time':
             self.wait_to_open_time = int(value)
         elif name == 'max-moves':
-            self.max_moves = 0
+            self.max_moves = int(value)
         elif name == 'initial-time':
-            self.initial_time = 0
+            self.initial_time = int(value)
 
     def configure(self, options: Dict[str, Union[str, int, bool]]) -> None:
         """Configure many options at once."""
         for name, value in options.items():
             self.setoption(name, value)
 
-    def _open_process(self, command: str, cwd: Optional[str] = None, shell: bool = True, _popen_lock: Any = threading.Lock()) -> subprocess.Popen:
+    def _open_process(self, command: str, cwd: Optional[str] = None, shell: bool = True,
+                      _popen_lock: Any = threading.Lock()) -> subprocess.Popen:
         """Open the engine process."""
         kwargs = {
             "shell": shell,
             "stdout": subprocess.PIPE,
             "stderr": subprocess.STDOUT,
             "stdin": subprocess.PIPE,
             "bufsize": 1,  # Line buffered
@@ -107,14 +110,16 @@
             try:
                 # Windows
                 logger.debug("Killing Windows.")
                 self.p.send_signal(signal.CTRL_BREAK_EVENT)
             except AttributeError:
                 # Unix
                 logger.debug("Killing UNIX.")
+                os.killpg(self.p.pid, signal.SIGTERM)
+                time.sleep(7)
                 os.killpg(self.p.pid, signal.SIGKILL)
 
             self.p.communicate()
             self.engine_receive_thread.join()
 
     def _connect(self) -> None:
         """Connect to the engine."""
@@ -124,19 +129,19 @@
             if wait_time > 0:
                 time.sleep(wait_time)
         self.sender.connect(self.ip, int(self.port))
 
     def _start(self, board: draughts.Board, game_time: int) -> None:
         """Start the game."""
         self._connect()
-        color = 'B' if board.turn == draughts.WHITE else 'W'
+        engine_color = 'B' if board.turn == draughts.WHITE else 'W'
         game_time = int(round(game_time // 60))
         moves = self.max_moves
         self.sender.setup(board.initial_fen, board.variant)
-        self.sender.gamereq(color, game_time, moves)
+        self.sender.gamereq(engine_color, game_time, moves)
         accepted = self._recv_accept()
         logger.debug(f'Aceepted: {accepted}')
         self.id["name"] = self.sender.current.engineName
 
     def _recv(self) -> None:
         """Receive a line from the engine, if the engine is opened by pydraughts."""
         # The engine doesn't work otherwise.
@@ -156,22 +161,56 @@
 
     def _recv_accept(self) -> bool:
         """Get if the game was accepted."""
         while True:
             if self.receiver.accepted is not None:
                 return self.receiver.accepted
 
-    def _recv_move(self) -> Optional[List[List[int]]]:
+    def _recv_move(self) -> Optional[draughts.Move]:
         """Receive the engine move."""
         while True:
             if not self.receiver.listening:
                 break
             if self.receiver.last_move_changed:
                 logger.debug(f'new last move: {self.receiver.last_move.board_move}')
                 return self.receiver.last_move
+        return None
+
+    def _recv_backreq(self) -> bool:
+        """Get if the backreq was accepted."""
+        while True:
+            if self.receiver.backreq_accepted is not None:
+                return self.receiver.backreq_accepted
+
+    def takeback(self, move: int, color: int) -> Tuple[bool, draughts.Board, Any]:
+        """
+        Attempt to take back moves.
+        Warning: If it is the engine's turn to play in the new position, it will attempt to move.
+        """
+        self.receiver.backreq_accepted = None
+        ply = (move - 1) * 2 + (0 if color == draughts.WHITE else 1)
+        remove_count = 0
+        best_move = None
+        moves = list(map(lambda old_move: old_move.steps_move, self.sender.current.pos.move_stack))
+        logger.debug(f"Move stack before removing: {moves}")
+        self.sender.backreq(move, color)
+        backreq = self._recv_backreq()
+        if backreq:
+            while len(self.sender.current.pos.move_stack) > ply:
+                remove_count += 1
+                self.sender.current.pos.pop()
+                moves = list(map(lambda old_move: old_move.steps_move, self.sender.current.pos.move_stack))
+                logger.debug(f"Move stack after removing {remove_count} moves: {moves}")
+            self.receiver.takeback_in_progress = False
+            new_board = self.sender.current.pos.copy()
+            if self.sender.current.engine_color == self.sender.current.get_color():  # It is the engine's turn to play.
+                best_move = self._recv_move()
+        else:
+            new_board = self.sender.current.pos.copy()
+        return backreq, new_board, draughts.engine.PlayResult(best_move, None, {})
 
     def play(self, board: draughts.Board) -> Any:
         """Engine search."""
         if not self.game_started:
             self._start(board, self.initial_time)
             self.game_started = True
         if board.move_stack:
```

### Comparing `pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_classes.py` & `pydraughts-0.6.4/draughts/engines/dxp_communication/dxp_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # This file is an adaptation of DXC100_draughts_client (https://github.com/akalverboer/DXC100_draughts_client) by akalverboer.
 
 from __future__ import annotations
 import socket
 import logging
 import draughts
+import time
 from typing import Dict, Optional, List, Union
 
 logger = logging.getLogger("pydraughts")
 
 DXP_WHITE = 0
 DXP_BLACK = 1
 
 
 class GameStatus:
-    def __init__(self, fen: str = 'startpos', my_color: int = DXP_WHITE, started: bool = False, variant: str = 'standard') -> None:
+    def __init__(self, fen: str = 'startpos', engine_color: int = DXP_WHITE, started: bool = False,
+                 variant: str = 'standard') -> None:
         self.fen = fen
-        self.my_color = my_color
+        self.engine_color = engine_color
         self.started = started
         self.variant = variant
         self.pos = draughts.Board(fen=fen, variant=variant)
         self.color = self.get_color()
         self.engineName = ''
         self.result = None
 
     def get_color(self) -> int:
         """Get the color of the playing side."""
         return DXP_WHITE if self.pos.turn == draughts.WHITE else DXP_BLACK
 
 
 class MySocket:
     def __init__(self) -> None:
-        self.sock = None
+        self.sock: Optional[socket.socket] = None
         self.closed = False
 
     def open(self) -> MySocket:
         """Open the socket."""
         try:
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
@@ -87,22 +89,23 @@
         msg = msg.replace("\0", "")  # remove all null chars
 
         # Use strip to remove all whitespace at the start and end.
         # Including spaces, tabs, newlines and carriage returns.
         msg = msg.strip()
         return msg
 
-    def close(self):
+    def close(self) -> None:
         if self.sock and not self.closed:
             self.closed = True
             self.sock.shutdown(socket.SHUT_RDWR)
+            time.sleep(7)
             self.sock.close()
             self.sock = None
 
-    def __del__(self):
+    def __del__(self) -> None:
         self.close()
 
 
 class DamExchange:
     def parse(self, msg: str) -> Dict[str, Union[str, List[str]]]:
         """Parse an incoming DXP message."""
         # Parse incoming DXP message. Returns relevant items depending on mtype.
@@ -152,15 +155,16 @@
 
     def msg_chat(self, msg: str) -> str:
         """Generate a CHAT message."""
         # Generate CHAT message. Example: CWhat do you think about move 35?
         msg = "C" + msg
         return msg
 
-    def msg_gamereq(self, my_color: int, game_time: int, num_moves: int, pos: Optional[draughts.Board] = None, color_to_move: Optional[int] = None) -> str:
+    def msg_gamereq(self, my_color: int, game_time: int, num_moves: int, pos: Optional[draughts.Board] = None,
+                    color_to_move: Optional[int] = None) -> str:
         """Generate a GAMEREQ message."""
         # Generate GAMEREQ message. Example: R01Tornado voor Windows 4.0        W060065A
         gamereq = []
         gamereq.append("R")  # header
         gamereq.append("01")  # version
 
         gamereq.append("DXP Client".ljust(32)[:32])  # iName: fixed length padding spaces
```

### Comparing `pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_communication.py` & `pydraughts-0.6.4/draughts/engines/dxp_communication/dxp_communication.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # This file is an adaptation of DXC100_draughts_client (https://github.com/akalverboer/DXC100_draughts_client) by akalverboer.
 
 from __future__ import annotations
 import threading
 import logging
 from draughts.engines.dxp_communication.dxp_classes import DamExchange, MySocket, GameStatus, DXP_WHITE, DXP_BLACK
-from draughts import Move
+from draughts import Move, WHITE
+from typing import Optional
 
 logger = logging.getLogger("pydraughts")
 
 
 class Receiver:
     def __init__(self, sender: Sender) -> None:
         self.sender = sender
-        self.accepted = None
+        self.accepted: Optional[bool] = None
         self.gameend_sent = False
-        self.last_move = None
+        self.last_move: Optional[Move] = None
         self.last_move_changed = False
         self.listening = False
         self.receive_thread_started = False
+        self.backreq_accepted: Optional[bool] = None
+        self.takeback_in_progress = False
         self.receive_thread = threading.Thread(target=self.receive)
-    
+
     def start(self) -> None:
         self.receive_thread_started = True
         self.receive_thread.start()
 
     def close(self) -> None:
         if self.receive_thread_started:
             self.receive_thread.join()
-    
-    def receive(self):
+
+    def receive(self) -> None:
         logger.debug("DXP Client starts listening")
         self.listening = True
         while True:
             try:
                 message = self.sender.socket.receive()  # wait for message
             except Exception as err:
                 logger.debug(f"Error {err}")
@@ -44,15 +47,15 @@
             if dxp_data["type"] == "C":
                 logger.debug(f"rcv CHAT: {message}")
                 logger.debug(f"\nChat message: {dxp_data['text']}")
 
             elif dxp_data["type"] == "A":
                 logger.debug(f"rcv GAMEACC: {message}")
                 if dxp_data["accCode"] == "0":
-                    self.sender.current.my_color = self.sender.current.my_color  # as requested
+                    self.sender.current.engine_color = self.sender.current.engine_color  # as requested
                     self.sender.current.engineName = dxp_data["engineName"]
                     logger.debug(f"\nGame request accepted by {dxp_data['engineName']}")
                     self.accepted = True
                     self.gameend_sent = False
                     self.sender.current.started = True
                 else:
                     logger.debug(f"\nGame request NOT accepted by {dxp_data['engineName']} Reason: {dxp_data['accCode']}")
@@ -61,39 +64,43 @@
 
             elif dxp_data["type"] == "E":
                 logger.debug(f"rcv GAMEEND: {message}")
                 logger.debug(f"\nRequest end of game accepted. Reason: {dxp_data['reason']} Stop: {dxp_data['stop']}")
                 # Confirm game end by sending message back (if not sent by me)
                 if self.sender.current.started and not self.gameend_sent:
                     self.sender.current.result = dxp_data["reason"]
-                    msg = self.sender.dxp.msg_gameend(dxp_data["reason"])
+                    msg = self.sender.dxp.msg_gameend(str(dxp_data["reason"]))  # `str` is there only for mypy.
                     self.sender.socket.send(msg)
                     logger.debug(f"snd GAMEEND: {msg}")
                     self.gameend_sent = True
                     self.sender.current.started = False
 
             elif dxp_data["type"] == "M":
                 logger.debug(f"rcv MOVE: {message}")
                 steps = [dxp_data['from'], dxp_data['to']]
                 nsteps = list(map(int, steps))
-                ntakes = list(map(int, dxp_data['captures']))
-                ntakes = list(map(lambda pos: str(pos).zfill(2), sorted(ntakes)))
+                ntakes_int = list(map(int, dxp_data['captures']))
+                ntakes = list(map(lambda pos: str(pos).zfill(2), sorted(ntakes_int)))
                 logger.debug(f"FEN: {self.sender.current.pos.fen}, Steps: {nsteps}, Takes: {ntakes}")
                 correct_move = None
+                while True:
+                    if not self.takeback_in_progress:
+                        break
                 for move in self.sender.current.pos.legal_moves():
                     if move.hub_position_move == f"{str(nsteps[0]).zfill(2)}{str(nsteps[-1]).zfill(2)}{''.join(ntakes)}":
                         correct_move = move
 
                 if correct_move is not None:
                     self.sender.current.pos.push(correct_move)
                     self.last_move = correct_move
                     logger.debug(f"Move received: {correct_move.steps_move}")
                     self.last_move_changed = True
                 else:
-                    logger.debug(f"Error: received move is illegal [{message}]\nMove history: {list(map(lambda old_move: old_move.steps_move, self.sender.current.pos.move_stack))}")
+                    move_history = list(map(lambda old_move: old_move.steps_move, self.sender.current.pos.move_stack))
+                    logger.debug(f"Error: received move is illegal [{message}]\nMove history: {move_history}")
 
             elif dxp_data["type"] == "B":
                 # For the time being do not confirm request from server: send message back.
                 logger.debug(f"rcv BACKREQ: {message}")
                 acc_code = "1"  # 0: BACK YES; 1: BACK NO; 2: CONTINUE
                 msg = self.sender.dxp.msg_backacc(acc_code)
                 self.sender.socket.send(msg)
@@ -102,35 +109,40 @@
             elif dxp_data["type"] == "K":
                 # Answer to my request to move back
                 logger.debug(f"rcv BACKACC: {message}")
                 logger.debug(f"rcv BACKACC: {message}")  # TEST
                 acc_code = dxp_data['accCode']
                 if acc_code == "0":
                     # Actions to go back in history as specified in my request
-                    raise NotImplementedError("Moving back is not implemented")
+                    self.backreq_accepted = True
+                elif acc_code == "1":
+                    logger.debug("Engine doesn't support going back.")
+                    self.backreq_accepted = False
+                else:
+                    logger.debug("Engine wants to continue the game.")
+                    self.backreq_accepted = False
 
             else:
                 logger.debug(f"rcv UNKNOWN: {message}")
                 logger.debug(f"\nrcv Unknown message: {message}")
 
         self.listening = False
 
 
 class Sender:
     def __init__(self) -> None:
         self.dxp = DamExchange()
         self.socket = MySocket()
-        self.game_status = GameStatus()
-        self.current = None
+        self.current = GameStatus("W")
         self.receiver = Receiver(self)
 
     def setup(self, fen: str, variant: str) -> None:
         logger.debug(f"FEN: {fen.strip()}, Variant: {variant}")
-        color = DXP_BLACK if fen[0] == 'B' else DXP_WHITE
-        self.current = GameStatus(fen=fen, my_color=color, variant=variant)
+        engine_color = DXP_BLACK if fen[0] == 'B' else DXP_WHITE
+        self.current = GameStatus(fen=fen, engine_color=engine_color, variant=variant)
 
     def send_move(self, move: Move) -> None:
         logger.debug(f"FEN: {self.current.pos.fen}, Steps: {move.steps_move}, Captures: {move.captures}")
         time_spent = 0
         self.receiver.last_move_changed = False
         self.current.pos.push(move)
         msg = self.dxp.msg_move(move.steps_move, move.captures, time_spent)
@@ -153,47 +165,54 @@
             return
         self.receiver.start()
 
     def disconnect(self) -> None:
         logger.debug("Attempting to disconnect.")
         try:
             self.socket.close()
-            logger.debug(f"Successfully closed socket.")
+            logger.debug("Successfully closed socket.")
         except Exception as err:
             self.socket.sock = None
             logger.debug(f"Error trying to close socket: {err}")
         self.receiver.close()
 
-    def chat(self, text: str):
+    def chat(self, text: str) -> None:
         text = text.strip()  # trim whitespace
         logger.debug(f"Text: {text}")
         msg = self.dxp.msg_chat(text)
         try:
             self.socket.send(msg)
             logger.debug(f"snd CHAT: {msg}")
         except Exception as err:
             logger.debug(f"Error sending chat message: {err}")
-            return
 
-    def gamereq(self, color: str, time: int, max_moves: int) -> None:
-        logger.debug(f"Color: {color}, Time: {time}, Max moves: {max_moves}")
-        dxp_color = DXP_WHITE if color.upper().startswith('W') else DXP_BLACK
+    def gamereq(self, engine_color: str, time: int, max_moves: int) -> None:
+        logger.debug(f"Engine color: {engine_color}, Time: {time}, Max moves: {max_moves}")
+        dxp_color = DXP_WHITE if engine_color.upper().startswith('W') else DXP_BLACK
         msg = self.dxp.msg_gamereq(dxp_color, time, max_moves, self.current.pos, self.current.get_color())
         try:
             self.socket.send(msg)
             logger.debug(f"snd GAMEREQ: {msg}")
         except Exception as err:
             logger.debug(f"Error sending game request: {err}")
-    
+
     def gameend(self) -> None:
         logger.debug("Attempting to send a gameend.")
         reason = "0"
         msg = self.dxp.msg_gameend(reason)
         self.receiver.gameend_sent = True
         try:
             self.socket.send(msg)
             logger.debug(f"snd GAMEEND: {msg}")
         except Exception as err:
             logger.debug(f"Error sending gameend message: {err}")
-    
-    def backreq(self) -> None:
-        raise NotImplementedError("Backreq isn't implemented yet.")
+
+    def backreq(self, move: int, color: int) -> None:
+        logger.debug(f"Request to return to {move}th move with {'WHITE' if color == WHITE else 'BLACK'} to move.")
+        msg = self.dxp.msg_backreq(move, DXP_WHITE if color == WHITE else DXP_BLACK)
+        self.receiver.last_move_changed = False
+        self.receiver.takeback_in_progress = True
+        try:
+            self.socket.send(msg)
+            logger.debug(f"snd BACKREQ: {msg}")
+        except Exception as err:
+            logger.debug(f"Error sending backreq request: {err}")
```

### Comparing `pydraughts-0.6.3/draughts/engines/hub.py` & `pydraughts-0.6.4/draughts/engines/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         command[0] = os.path.realpath(os.path.expanduser(command[0]))
         command[0] = '"' + command[0] + '"'
         command = ' '.join(command)
         self.p = self._open_process(command, cwd)
         self._last_sent = ""
         self.hub()
 
-    def _open_process(self, command: str, cwd: Optional[str] = None, shell: Optional[bool] = True, _popen_lock: Any = threading.Lock()) -> subprocess.Popen:
+    def _open_process(self, command: str, cwd: Optional[str] = None, shell: Optional[bool] = True,
+                      _popen_lock: Any = threading.Lock()) -> subprocess.Popen:
         """Open the engine process."""
         kwargs: Dict[str, Any] = {
             "shell": shell,
             "stdout": subprocess.PIPE,
             "stderr": subprocess.STDOUT,
             "stdin": subprocess.PIPE,
             "bufsize": 1,  # Line buffered
@@ -97,14 +98,15 @@
     def recv_hub(self) -> List[str]:
         """Receive a line from the engine and split at the first space."""
         command_and_args = self.recv().split(None, 1)
         if len(command_and_args) == 1:
             return [command_and_args[0], ""]
         elif len(command_and_args) == 2:
             return command_and_args
+        return []
 
     def hub(self) -> Tuple[Dict[str, str], Set[str], Set[str]]:
         """Send the hub command to an engine."""
         self.send("hub")
 
         engine_info: Dict[str, str] = {}
         options: Set[str] = set()
@@ -175,15 +177,18 @@
             self.send("set-param name=%s value=%s" % (name, value))
 
     def configure(self, options: Dict[str, Union[str, bool, None]]) -> None:
         """Configure many options at once."""
         for name, value in options.items():
             self.setoption(name, value)
 
-    def go(self, fen: str, moves: Optional[str] = None, my_time: Union[int, float, None] = None, inc: Union[int, float, None] = None, moves_left: Optional[int] = None, movetime: Union[int, float, None] = None, depth: Optional[int] = None, nodes: Optional[int] = None, ponder: Optional[bool] = False) -> Tuple[str, Optional[str]]:
+    def go(self, fen: str, moves: Optional[str] = None, my_time: Union[int, float, None] = None,
+           inc: Union[int, float, None] = None, moves_left: Optional[int] = None,
+           movetime: Union[int, float, None] = None, depth: Optional[int] = None, nodes: Optional[int] = None,
+           ponder: Optional[bool] = False) -> Tuple[str, Optional[str]]:
         """Send the engine a go command."""
         if moves:
             self.send(f'pos pos={fen} moves="{moves}"')
         else:
             self.send(f'pos pos={fen}')
 
         if my_time is not None and inc and moves_left:
@@ -258,17 +263,17 @@
     def play(self, board: draughts.Board, time_limit: Any, ponder: bool) -> Any:
         """Engine search."""
         time = time_limit.time
         inc = time_limit.inc
         depth = time_limit.depth
         nodes = time_limit.nodes
         movetime = time_limit.movetime
-        hub_moves = board.move_stack
-        hub_moves = list(map(lambda move: move.hub_move, hub_moves))
-        bestmove, pondermove = self.go(board._game.initial_hub_fen, moves=' '.join(hub_moves), my_time=time, inc=inc, depth=depth, nodes=nodes, movetime=movetime, ponder=ponder)
+        hub_moves = list(map(lambda move: move.hub_move, board.move_stack))
+        bestmove, pondermove = self.go(board._game.initial_hub_fen, moves=' '.join(hub_moves), my_time=time, inc=inc,
+                                       depth=depth, nodes=nodes, movetime=movetime, ponder=ponder)
 
         ponder_move = None
         ponder_board = board.copy()
         best_move = draughts.Move(ponder_board, hub_move=bestmove)
         if pondermove:
             ponder_board.push(best_move)
             ponder_move = draughts.Move(ponder_board, hub_move=pondermove)
```

### Comparing `pydraughts-0.6.3/other_licenses/ImparaAI checkers LICENSE` & `pydraughts-0.6.4/other_licenses/ImparaAI checkers LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/other_licenses/akalverboer DXC100_draughts_client LICENSE` & `pydraughts-0.6.4/other_licenses/akalverboer DXC100_draughts_client LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/other_licenses/fishnet LICENSE.txt` & `pydraughts-0.6.4/other_licenses/fishnet LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.3/pydraughts.egg-info/PKG-INFO` & `pydraughts-0.6.4/pydraughts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.3
+Version: 0.6.4
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
 Author: Ioannis Pantidis
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -139,14 +139,25 @@
 * Get a ballot
 ```python
 from draughts.ballots import Ballots
 ballots = Ballots('english')
 ballot1 = ballots.get_ballot()
 ballot2 = ballots.get_ballot()
 ```
+* Run tournaments
+```python
+from draughts.tournament import RoundRobin
+player1 = (["scan.exe", "hub"], "hub", {})
+player2 = ("kr_hub.exe", "hub", {})
+players = [player1, player2]
+tournament = RoundRobin("tournament.pdn", players, start_time=20, increment=0.2, games_per_pair=4)
+scores = tournament.play()
+print(scores)
+tournament.print_standings()
+```
 
 ## Acknowledgements
 Thanks to [fishnet](https://github.com/lichess-org/fishnet/tree/ebd2a5e16d37135509cbfbff9998e0b798866ef5) which was modified to add support for Hub engines. Thanks to [akalverboer](https://github.com/akalverboer) for their [DXC100_draughts_client](https://github.com/akalverboer/DXC100_draughts_client) which was modified to add support for DXP engines.
 
 ## License
 pydraughts is licensed under The MIT License. Check out `LICENSE` for the full text.
 The licenses of the other projects that pydraughts uses are in the `other_licenses` folder.
```

### Comparing `pydraughts-0.6.3/pydraughts.egg-info/SOURCES.txt` & `pydraughts-0.6.4/pydraughts.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 draughts/PDN.py
 draughts/__init__.py
 draughts/ballots.py
 draughts/convert.py
 draughts/engine.py
+draughts/tournament.py
 draughts/ballot_files/11_english.json
 draughts/ballot_files/11_italian.json
 draughts/ballot_files/150russian_and_brazilian.json
 draughts/ballot_files/2move_english.json
 draughts/ballot_files/3move_english.json
 draughts/ballot_files/4move_english.json
 draughts/ballot_files/5move_english.json
@@ -33,15 +34,14 @@
 draughts/engines/checkerboard_extra/engine_64.py
 draughts/engines/checkerboard_extra/engine_client.py
 draughts/engines/checkerboard_extra/engine_server.py
 draughts/engines/checkerboard_extra/get_checker_board.py
 draughts/engines/dxp_communication/__init__.py
 draughts/engines/dxp_communication/dxp_classes.py
 draughts/engines/dxp_communication/dxp_communication.py
-draughts/engines/dxp_communication/dxp_run.py
 other_licenses/ImparaAI checkers LICENSE
 other_licenses/akalverboer DXC100_draughts_client LICENSE
 other_licenses/fishnet LICENSE.txt
 pydraughts.egg-info/PKG-INFO
 pydraughts.egg-info/SOURCES.txt
 pydraughts.egg-info/dependency_links.txt
 pydraughts.egg-info/requires.txt
```

### Comparing `pydraughts-0.6.3/setup.cfg` & `pydraughts-0.6.4/setup.cfg`

 * *Files identical despite different names*

