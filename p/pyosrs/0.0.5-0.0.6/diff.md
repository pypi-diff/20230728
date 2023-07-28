# Comparing `tmp/pyosrs-0.0.5.tar.gz` & `tmp/pyosrs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosrs-0.0.5.tar", max compression
+gzip compressed data, was "pyosrs-0.0.6.tar", max compression
```

## Comparing `pyosrs-0.0.5.tar` & `pyosrs-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-06-18 17:03:43.880676 pyosrs-0.0.5/LICENSE
--rw-r--r--   0        0        0     2473 2023-06-18 17:03:43.884676 pyosrs-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/__init__.py
--rw-r--r--   0        0        0     6423 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/client.py
--rw-r--r--   0        0        0     4835 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/enums.py
--rw-r--r--   0        0        0      410 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/exceptions.py
--rw-r--r--   0        0        0     4002 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/models.py
--rw-r--r--   0        0        0      901 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyosrs/utils.py
--rw-r--r--   0        0        0      767 2023-06-18 17:03:43.884676 pyosrs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 pyosrs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-07-28 20:28:22.164941 pyosrs-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2473 2023-07-28 20:28:22.164941 pyosrs-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/__init__.py
+-rw-r--r--   0        0        0     6423 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/client.py
+-rw-r--r--   0        0        0     4912 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/enums.py
+-rw-r--r--   0        0        0      410 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/exceptions.py
+-rw-r--r--   0        0        0     4162 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/models.py
+-rw-r--r--   0        0        0      901 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyosrs/utils.py
+-rw-r--r--   0        0        0      767 2023-07-28 20:28:22.164941 pyosrs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 pyosrs-0.0.6/PKG-INFO
```

### Comparing `pyosrs-0.0.5/LICENSE` & `pyosrs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.5/README.md` & `pyosrs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.5/pyosrs/client.py` & `pyosrs-0.0.6/pyosrs/client.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.5/pyosrs/enums.py` & `pyosrs-0.0.6/pyosrs/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,21 +49,21 @@
     36: ("lms", "LMS"),
     37: ("pvp_arena", "PvP Arena"),
     38: ("soul_wars", "Soul Wars Zeal"),
     39: ("rifts_closed", "Rifts Closed"),
 }
 
 CLUES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
-    29: ("clue_scrolls_all", "Clue Scrolls All"),
-    30: ("clue_scrolls_beginner", "Clue Scrolls Beginner"),
-    31: ("clue_scrolls_easy", "Clue Scrolls Easy"),
-    32: ("clue_scrolls_medium", "Clue Scrolls Medium"),
-    33: ("clue_scrolls_hard", "Clue Scrolls Hard"),
-    34: ("clue_scrolls_elite", "Clue Scrolls Elite"),
-    35: ("clue_scrolls_master", "Clue Scrolls Master"),
+    29: ("all", "Clue Scrolls All"),
+    30: ("beginner", "Clue Scrolls Beginner"),
+    31: ("easy", "Clue Scrolls Easy"),
+    32: ("medium", "Clue Scrolls Medium"),
+    33: ("hard", "Clue Scrolls Hard"),
+    34: ("elite", "Clue Scrolls Elite"),
+    35: ("master", "Clue Scrolls Master"),
 }
 
 BOSSES_INDEX: Final[Dict[int, Tuple[str, str]]] = {
     40: ("abyssal_sire", "Abyssal Sire"),
     41: ("alchemical_hydra", "Alchemical Hydra"),
     42: ("artio", "Artio"),
     43: ("barrows_chests", "Barrows Chests"),
@@ -81,47 +81,51 @@
     52: ("commander_zilyana", "Commander Zilyana"),
     53: ("corporeal_beast", "Corporeal Beast"),
     54: ("crazy_archaeologist", "Crazy Archaeologist"),
     55: ("dagannoth_prime", "Dagannoth Prime"),
     56: ("dagannoth_rex", "Dagannoth Rex"),
     57: ("dagannoth_supreme", "Dagannoth Supreme"),
     58: ("deranged_archaeologist", "Deranged Archaeologist"),
-    59: ("general_graardor", "General Graardor"),
-    60: ("giant_mole", "Giant Mole"),
-    61: ("grotesque_guardians", "Grotesque Guardians"),
-    62: ("hespori", "Hespori"),
-    63: ("kalphite_queen", "Kalphite Queen"),
-    64: ("king_black_dragon", "King Black Dragon"),
-    65: ("kraken", "Kraken"),
-    66: ("kree_arra", "Kree'Arra"),
-    67: ("kril_tsutsaroth", "K'ril Tsutsaroth"),
-    68: ("mimic", "Mimic"),
-    69: ("nex", "Nex"),
-    70: ("nightmare", "Nightmare"),
-    71: ("phosanis_nightmare", "Phosani's Nightmare"),
-    72: ("obor", "Obor"),
-    73: ("phantom_muspah", "Phantom Muspah"),
-    74: ("sarachnis", "Sarachnis"),
-    75: ("scorpia", "Scorpia"),
-    76: ("skotizo", "Skotizo"),
-    77: ("spindel", "Spindel"),
-    78: ("tempoross", "Tempoross"),
-    79: ("the_gauntlet", "The Gauntlet"),
-    80: ("the_corrupted_gauntlet", "The Corrupted Gauntlet"),
-    81: ("theatre_of_blood", "Theatre of Blood"),
-    82: ("theatre_of_blood_hard_mode", "Theatre of Blood: Hard Mode"),
-    83: ("thermonuclear_smoke_devil", "Thermonuclear Smoke Devil"),
-    84: ("tombs_of_amascut", "Tombs of Amascut"),
-    85: ("tombs_of_amascut_expert_mode", "Tombs of Amascut: Expert Mode"),
-    86: ("tzkal_zuk", "TzKal-Zuk"),
-    87: ("tztok_jad", "TzTok-Jad"),
-    88: ("venenatis", "Venenatis"),
-    89: ("vet_ion", "Vet'ion"),
-    90: ("vorkath", "Vorkath"),
-    91: ("wintertodt", "Wintertodt"),
-    92: ("zalcano", "Zalcano"),
-    93: ("zulrah", "Zulrah"),
+    59: ("duke_sucellus", "Duke Sucellus"),
+    60: ("general_graardor", "General Graardor"),
+    61: ("giant_mole", "Giant Mole"),
+    62: ("grotesque_guardians", "Grotesque Guardians"),
+    63: ("hespori", "Hespori"),
+    64: ("kalphite_queen", "Kalphite Queen"),
+    65: ("king_black_dragon", "King Black Dragon"),
+    66: ("kraken", "Kraken"),
+    67: ("kree_arra", "Kree'Arra"),
+    68: ("kril_tsutsaroth", "K'ril Tsutsaroth"),
+    69: ("mimic", "Mimic"),
+    70: ("nex", "Nex"),
+    71: ("nightmare", "Nightmare"),
+    72: ("phosanis_nightmare", "Phosani's Nightmare"),
+    73: ("obor", "Obor"),
+    74: ("phantom_muspah", "Phantom Muspah"),
+    75: ("sarachnis", "Sarachnis"),
+    76: ("scorpia", "Scorpia"),
+    77: ("skotizo", "Skotizo"),
+    78: ("spindel", "Spindel"),
+    79: ("tempoross", "Tempoross"),
+    80: ("the_gauntlet", "The Gauntlet"),
+    81: ("the_corrupted_gauntlet", "The Corrupted Gauntlet"),
+    82: ("the_leviathan", "The Leviathan"),
+    83: ("the_whisperer", "The Whisperer"),
+    84: ("theatre_of_blood", "Theatre of Blood"),
+    85: ("theatre_of_blood_hard_mode", "Theatre of Blood: Hard Mode"),
+    86: ("thermonuclear_smoke_devil", "Thermonuclear Smoke Devil"),
+    87: ("tombs_of_amascut", "Tombs of Amascut"),
+    88: ("tombs_of_amascut_expert_mode", "Tombs of Amascut: Expert Mode"),
+    89: ("tzkal_zuk", "TzKal-Zuk"),
+    90: ("tztok_jad", "TzTok-Jad"),
+    91: ("vardorvis", "Vardorvis"),
+    92: ("venenatis", "Venenatis"),
+    93: ("vet_ion", "Vet'ion"),
+    94: ("vorkath", "Vorkath"),
+    95: ("wintertodt", "Wintertodt"),
+    96: ("zalcano", "Zalcano"),
+    97: ("zulrah", "Zulrah"),
 }
 
 HISCORE_RESPONSE_LEN: Final[int] = (
     len(SKILLS_INDEX) + len(MINIGAMES_INDEX) + len(CLUES_INDEX) + len(BOSSES_INDEX)
 )
```

### Comparing `pyosrs-0.0.5/pyosrs/models.py` & `pyosrs-0.0.6/pyosrs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     commander_zilyana: Minigame = Minigame()
     corporeal_beast: Minigame = Minigame()
     crazy_archaeologist: Minigame = Minigame()
     dagannoth_prime: Minigame = Minigame()
     dagannoth_rex: Minigame = Minigame()
     dagannoth_supreme: Minigame = Minigame()
     deranged_archaeologist: Minigame = Minigame()
+    duke_sucellus: Minigame = Minigame()
     general_graardor: Minigame = Minigame()
     giant_mole: Minigame = Minigame()
     grotesque_guardians: Minigame = Minigame()
     hespori: Minigame = Minigame()
     kalphite_queen: Minigame = Minigame()
     king_black_dragon: Minigame = Minigame()
     kraken: Minigame = Minigame()
@@ -100,21 +101,24 @@
     sarachnis: Minigame = Minigame()
     scorpia: Minigame = Minigame()
     skotizo: Minigame = Minigame()
     spindel: Minigame = Minigame()
     tempoross: Minigame = Minigame()
     the_gauntlet: Minigame = Minigame()
     the_corrupted_gauntlet: Minigame = Minigame()
+    the_leviathan: Minigame = Minigame()
+    the_whisperer: Minigame = Minigame()
     theatre_of_blood: Minigame = Minigame()
     theatre_of_blood_hard_mode: Minigame = Minigame()
     thermonuclear_smoke_devil: Minigame = Minigame()
     tombs_of_amascut: Minigame = Minigame()
     tombs_of_amascut_expert_mode: Minigame = Minigame()
     tzkal_zuk: Minigame = Minigame()
     tztok_jad: Minigame = Minigame()
+    vardorvis: Minigame = Minigame()
     venenatis: Minigame = Minigame()
     vet_ion: Minigame = Minigame()
     vorkath: Minigame = Minigame()
     wintertodt: Minigame = Minigame()
     zalcano: Minigame = Minigame()
     zulrah: Minigame = Minigame()
```

### Comparing `pyosrs-0.0.5/pyosrs/utils.py` & `pyosrs-0.0.6/pyosrs/utils.py`

 * *Files identical despite different names*

### Comparing `pyosrs-0.0.5/pyproject.toml` & `pyosrs-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyosrs"
-version = "0.0.5"
+version = "0.0.6"
 description = "A Python library for Oldschool RuneScape."
 authors = ["Phong Tran"]
 repository = "https://github.com/phongse/pyosrs"
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pyosrs-0.0.5/PKG-INFO` & `pyosrs-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosrs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python library for Oldschool RuneScape.
 Home-page: https://github.com/phongse/pyosrs
 License: LGPL-3.0-only
 Author: Phong Tran
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

