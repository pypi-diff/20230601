# Comparing `tmp/hearthstone-6.7.0.tar.gz` & `tmp/hearthstone-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-6.7.0.tar", last modified: Tue May  9 22:22:31 2023, max compression
+gzip compressed data, was "hearthstone-6.8.0.tar", last modified: Wed May 31 22:11:09 2023, max compression
```

## Comparing `hearthstone-6.7.0.tar` & `hearthstone-6.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:22:31.775219 hearthstone-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-09 22:22:25.000000 hearthstone-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-09 22:22:31.775219 hearthstone-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-09 22:22:25.000000 hearthstone-6.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:22:31.771219 hearthstone-6.7.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    59191 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:22:31.775219 hearthstone-6.7.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 22:22:25.000000 hearthstone-6.7.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:22:31.775219 hearthstone-6.7.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:22:31.000000 hearthstone-6.7.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 22:22:31.775219 hearthstone-6.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-09 22:22:25.000000 hearthstone-6.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:11:09.505477 hearthstone-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 22:11:04.000000 hearthstone-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-31 22:11:09.505477 hearthstone-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 22:11:04.000000 hearthstone-6.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:11:09.505477 hearthstone-6.8.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59267 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:11:09.505477 hearthstone-6.8.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-31 22:11:04.000000 hearthstone-6.8.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:11:09.505477 hearthstone-6.8.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:11:09.000000 hearthstone-6.8.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 22:11:09.505477 hearthstone-6.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-31 22:11:04.000000 hearthstone-6.8.0/setup.py
```

### Comparing `hearthstone-6.7.0/LICENSE` & `hearthstone-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/PKG-INFO` & `hearthstone-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.7.0
+Version: 6.8.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.7.0/README.md` & `hearthstone-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/bountyxml.py` & `hearthstone-6.8.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/cardxml.py` & `hearthstone-6.8.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/dbf.py` & `hearthstone-6.8.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/deckstrings.py` & `hearthstone-6.8.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/entities.py` & `hearthstone-6.8.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/enums.py` & `hearthstone-6.8.0/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,15 @@
 	USE_FAST_ACTOR_TRANSITION_ANIMATIONS = 1402
 	DECK_RULE_COUNT_AS_COPY_OF_CARD_ID = 1413
 	STUDY = 1414
 	BACON_ODD_PLAYER_OUT = 1415
 	BACON_IS_KEL_THUZAD = 1423
 	HIGHLIGHT_ATTACKING_MINION_DURING_COMBAT = 1424
 	SPELLBURST = 1427
+	BACON_TRIPLE_UPGRADE_MINION_ID = 1429
 	RULEBOOK = 1430
 	FX_DATANUM_1 = 1436
 	BACON_ACTION_CARD = 1437
 	GAME_MODE_BUTTON_SLOT = 1438
 	TECH_LEVEL = 1440
 	TECH_LEVEL_MANA_GEM = 1442
 	UI_BUFF_DURABILITY_UP = 1443
@@ -459,14 +460,15 @@
 	COLLECTION_RELATED_CARD_DATABASE_ID = 1452
 	IS_BACON_POOL_MINION = 1456
 	SUPPRESS_ALL_SUMMON_VO = 1458
 	BACON_TRIPLE_CANDIDATE = 1460
 	BATTLEGROUNDS_PREMIUM_EMOTES = 1463
 	MOVE_MINION_HOVER_TARGET_SLOT = 1464
 	BACON_COIN_ON_ENEMY_MINIONS = 1467
+	BACON_TRIPLED_BASE_MINION_ID = 1471
 	ALWAYS_USE_FAST_ACTOR_TRIGGERS = 1473
 	PIECE_OF_CTHUN = 1477
 	BACON_HERO_CAN_BE_DRAFTED = 1491
 	TRANSIENT_ENTITY = 1493
 	DISABLE_NONHERO_GOLDEN_ANIMATIONS = 1514
 	WATERMARK_OVERRIDE_CARD_SET = 1517
 	DORMANT = 1518
```

### Comparing `hearthstone-6.7.0/hearthstone/mercenaryxml.py` & `hearthstone-6.8.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/stringsfile.py` & `hearthstone-6.8.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone/utils/__init__.py` & `hearthstone-6.8.0/hearthstone/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -363,14 +363,39 @@
 	"BAR_914t2": "BAR_914",
 	# Harmonic / Dissonant cards
 	"ETC_314t": "ETC_314",  # Harmonic Pop
 	"ETC_379t": "ETC_379",  # Harmonic Mood
 	"ETC_427t": "ETC_427",  # Harmonic Metal
 	"ETC_506t": "ETC_506",  # Harmonic Disco
 	"ETC_717t": "ETC_717",  # Harmonic Hip Hop
+	# Remixed Dispense-o-bot
+	"JAM_000t": "JAM_000",  # Chilling Dispense-o-bot
+	"JAM_000t2": "JAM_000",  # Merch Dispense-o-bot
+	"JAM_000t3": "JAM_000",  # Money Dispense-o-bot
+	"JAM_000t4": "JAM_000",  # Mystery Dispense-o-bot
+	# Remixed Totemcarver
+	"JAM_012t": "JAM_012",  # Loud Totemcarver
+	"JAM_012t2": "JAM_012",  # Bluesy Totemcarver
+	"JAM_012t3": "JAM_012",  # Blazing Totemcarver
+	"JAM_012t4": "JAM_012",  # Karaoke Totemcarver
+	# Remixed Tuning Fork
+	"JAM_015t": "JAM_015",  # Sharpened Tuning Fork
+	"JAM_015t2": "JAM_015",  # Reinforced Tuning Fork
+	"JAM_015t3": "JAM_015",  # Curved Tuning Fork
+	"JAM_015t4": "JAM_015",  # Backup Tuning Fork
+	# Remixed Rhapsody
+	"JAM_018t": "JAM_018",  # Angsty Rhapsody
+	"JAM_018t2": "JAM_018",  # Resounding Rhapsody
+	"JAM_018t3": "JAM_018",  # Emotional Rhapsody
+	"JAM_018t4": "JAM_018",  # Wailing Rhapsody
+	# Remixed Musician
+	"JAM_033t": "JAM_033",  # Cathedral Musician
+	"JAM_033t2": "JAM_033",  # Tropical Musician
+	"JAM_033t3": "JAM_033",  # Romantic Musician
+	"JAM_033t4": "JAM_033",  # Noise Musician
 }
 
 
 def get_original_card_id(card_id):
 	# Transfer Student
 	if str(card_id).startswith("SCH_199t"):
 		return "SCH_199"
```

### Comparing `hearthstone-6.7.0/hearthstone/xmlutils.py` & `hearthstone-6.8.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-6.8.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.7.0
+Version: 6.8.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.7.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-6.8.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-6.7.0/setup.cfg` & `hearthstone-6.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 6.7.0
+version = 6.8.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

