# Comparing `tmp/pmdsky_debug_py-7.0.6-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 885527 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-30 04:23 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-30 04:23 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   754662 b- defN 23-Jul-30 04:23 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   720673 b- defN 23-Jul-30 04:23 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   741723 b- defN 23-Jul-30 04:23 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   720673 b- defN 23-Jul-30 04:23 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   762044 b- defN 23-Jul-30 04:23 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   720684 b- defN 23-Jul-30 04:23 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   253000 b- defN 23-Jul-30 04:23 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 04:23 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-30 04:23 pmdsky_debug_py-7.0.6.dist-info/RECORD
-14 files, 4677903 bytes uncompressed, 883629 bytes compressed:  81.1%
+Zip file size: 886611 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Aug-01 04:24 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Aug-01 04:24 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   755146 b- defN 23-Aug-01 04:24 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   721145 b- defN 23-Aug-01 04:24 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   742195 b- defN 23-Aug-01 04:24 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   721145 b- defN 23-Aug-01 04:24 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   762528 b- defN 23-Aug-01 04:24 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   721156 b- defN 23-Aug-01 04:24 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   253065 b- defN 23-Aug-01 04:24 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 04:24 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/RECORD
+14 files, 4680824 bytes uncompressed, 884713 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.6.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.6.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.6.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.6.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+13fdd590a2"
+RELEASE = "v0.7.0+8f9ddefb60"
```

## pmdsky_debug_py/eu.py

```diff
@@ -5756,14 +5756,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        [0x66098],
+        [0x2066098],
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         [0x6AAAC],
         [0x206AAAC],
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10551,21 +10559,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         [0x5E24],
         [0x22C31E4],
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class EuOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         [0x79A4],
         [0x22C4D64],
@@ -20694,18 +20705,18 @@
     )
 
     RunDungeonMode = Symbol(
         [0x6FFA8],
         [0x234CB28],
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         [0x70F70],
         [0x234DAF0],
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -5564,14 +5564,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        None,
+        None,
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         None,
         None,
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10293,21 +10301,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         None,
         None,
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class EuItcmOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         None,
         None,
@@ -20189,18 +20200,18 @@
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         None,
         None,
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/jp.py

```diff
@@ -5754,14 +5754,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        None,
+        None,
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         [0x6AA08],
         [0x206AA08],
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10521,21 +10529,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         [0x5D54],
         [0x22C3F74],
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class JpOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         None,
         None,
@@ -20448,18 +20459,18 @@
     )
 
     RunDungeonMode = Symbol(
         [0x6F8AC],
         [0x234D18C],
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         [0x70874],
         [0x234E154],
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -5564,14 +5564,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        None,
+        None,
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         None,
         None,
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10293,21 +10301,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         None,
         None,
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class JpItcmOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         None,
         None,
@@ -20189,18 +20200,18 @@
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         None,
         None,
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/na.py

```diff
@@ -5756,14 +5756,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        [0x65D1C],
+        [0x2065D1C],
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         [0x6A714],
         [0x206A714],
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10559,21 +10567,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         [0x5E0C],
         [0x22C288C],
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class NaOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         [0x798C],
         [0x22C440C],
@@ -20778,18 +20789,18 @@
     )
 
     RunDungeonMode = Symbol(
         [0x6FCE8],
         [0x234BF28],
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         [0x70CB0],
         [0x234CEF0],
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -5564,14 +5564,22 @@
         None,
         "Gets info about the item at a given item table (not sure what this table"
         " is...) index.\n\nUsed by SPECIAL_PROC_COUNT_TABLE_ITEM_TYPE_IN_BAG and"
         " friends (see ScriptSpecialProcessCall).\n\nr0: table index\nr1: [output]"
         " pointer to an owned_item",
     )
 
+    MainLoop = Symbol(
+        None,
+        None,
+        None,
+        "This function gets called shortly after the game is started. Contains a single"
+        " infinite loop and has no return statement.\n\nNo params.",
+    )
+
     DungeonSwapIdToIdx = Symbol(
         None,
         None,
         None,
         "Converts a dungeon ID to its corresponding index in DUNGEON_SWAP_ID_TABLE, or"
         " -1 if not found.\n\nr0: dungeon ID\nreturn: index",
     )
@@ -10293,21 +10301,24 @@
         None,
         "Given a tileset ID, returns whether it's a background or a regular"
         " tileset\n\nIn particular, returns r0 >= 0xAA\n\nr0: Tileset ID\nreturn: True"
         " if the tileset ID corresponds to a background, false if it corresponds to a"
         " regular tileset",
     )
 
-    CheckEndDungeon = Symbol(
+    MainGame = Symbol(
         None,
         None,
         None,
-        "Do the stuff when you lose in a dungeon.\n\nNote: unverified, ported from"
-        " Irdkwia's notes\n\nr0: End condition code? Seems to control what tasks get"
-        " run and what transition happens when the dungeon ends\nreturn: return code?",
+        "Contains several functions that handle switching between ground and dungeon"
+        " mode. It also handles other situations, like what happens right after exiting"
+        " a dungeon.\n\nThe function doesn't get called until the player selects the"
+        " option to resume a saved game and doesn't return until the player returns to"
+        " the main menu.\n\nr0: End condition code? Seems to control what tasks get run"
+        " and what transition happens when the dungeon ends\nreturn: return code?",
     )
 
 
 class NaItcmOverlay10Data:
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS = Symbol(
         None,
         None,
@@ -20189,18 +20200,18 @@
     )
 
     RunDungeonMode = Symbol(
         None,
         None,
         None,
         "This appears to be the top-level function for running dungeon mode.\n\nIt gets"
-        " called by some code in overlay 10 right after doing the dungeon fade"
-        " transition, and once it exits, the dungeon results are processed.\n\nThis"
-        " function is presumably in charge of allocating the dungeon struct, setting it"
-        " up, launching the dungeon engine, etc.",
+        " called by MainGame right after doing the dungeon fade transition, and once it"
+        " exits, the dungeon results are processed.\n\nThis function is presumably in"
+        " charge of allocating the dungeon struct, setting it up, launching the dungeon"
+        " engine, etc.",
     )
 
     DisplayDungeonTip = Symbol(
         None,
         None,
         None,
         "Checks if a given dungeon tip should be displayed at the start of a floor and"
```

## pmdsky_debug_py/protocol.py

```diff
@@ -3562,14 +3562,19 @@
     ]
 
     ItemAtTableIdx: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    MainLoop: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DungeonSwapIdToIdx: Symbol[
         Optional[List[int]],
         None,
     ]
 
     DungeonSwapIdxToId: Symbol[
         Optional[List[int]],
@@ -6629,15 +6634,15 @@
     ]
 
     IsBackgroundTileset: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    CheckEndDungeon: Symbol[
+    MainGame: Symbol[
         Optional[List[int]],
         None,
     ]
 
 
 class Overlay10DataProtocol(Protocol):
     FIRST_DUNGEON_WITH_MONSTER_HOUSE_TRAPS: Symbol[
```

## Comparing `pmdsky_debug_py-7.0.6.dist-info/METADATA` & `pmdsky_debug_py-7.0.7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.6
+Version: 7.0.7
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `pmdsky_debug_py-7.0.6.dist-info/RECORD` & `pmdsky_debug_py-7.0.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pmdsky_debug_py/__init__.py,sha256=xvXjdxEqeoQaaS6ssZYVI9jARzv5M4q6FNwA3Z6fOw4,1831
-pmdsky_debug_py/_release.py,sha256=0VDqIaCuXrUgsCjUjn7piH3KNmUoS6_zPc9CjcRG2K8,30
-pmdsky_debug_py/eu.py,sha256=m9-ruyMm6nfPCvX17TDZdCxVGKSiARWtFrJvdK3sTFI,754662
-pmdsky_debug_py/eu_itcm.py,sha256=hPhv_xn6x5naumBVSm1rIQrhiUVzLvhvBSMC5LwoHYo,720673
-pmdsky_debug_py/jp.py,sha256=IO6-flBoTliws1ryrCQ__ARdHCE8ZqvSlZT6be_Ix98,741723
-pmdsky_debug_py/jp_itcm.py,sha256=QDVLPj65CCeJ_Motw993bvmP9r7-c06V9FrXQmkQtE4,720673
-pmdsky_debug_py/na.py,sha256=1OzuuqT2WUSCsxF818jw2YH60MwNU6E6ul5GORXMlf4,762044
-pmdsky_debug_py/na_itcm.py,sha256=ghKwXSsBXPOI6qwmcr4CGUUKgdKPBKcsWte8XM3iJVs,720684
-pmdsky_debug_py/protocol.py,sha256=whT4-RmbrQC8X8tr6pXBqgR2BiAS-IY9bHg5MBS8_dQ,253000
+pmdsky_debug_py/_release.py,sha256=PsVd5GQn9fUVLX148VsfjNdVxOlS56gso6_2lUa12T8,30
+pmdsky_debug_py/eu.py,sha256=3aHXO74NfXBnPHmKWHFnNYxJqxj8fL_yasXj8pdEFm0,755146
+pmdsky_debug_py/eu_itcm.py,sha256=klJPKVIsIziBm6o4zpZ6EhhG9krcQ923vvFsJQR5Tzc,721145
+pmdsky_debug_py/jp.py,sha256=nYs5Bb9_NJyKvTwieUh83E2mkbCfuI8OLLcd8kQDNEw,742195
+pmdsky_debug_py/jp_itcm.py,sha256=JSsYrR_IfZavqDeYbMNh1dByPK9KPIQrcfQLMOEq2KM,721145
+pmdsky_debug_py/na.py,sha256=i34tcIZrL8FNm-XRFtaMoH_FfZr3-y2yrE2vGUSym24,762528
+pmdsky_debug_py/na_itcm.py,sha256=F-2C0HDdx18sRXg45-ZUGlCKwW4CpeI0QPgDnAMnnwM,721156
+pmdsky_debug_py/protocol.py,sha256=60ssOgw2ijN0Di9wmHaK7bD8qJQL01MfBT2QTiODL8s,253065
 pmdsky_debug_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pmdsky_debug_py-7.0.6.dist-info/METADATA,sha256=v-40PIzA2HGtJQtEEMB2LST2U-HCA2sDCgl-RDxw1Fk,1320
-pmdsky_debug_py-7.0.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pmdsky_debug_py-7.0.6.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
-pmdsky_debug_py-7.0.6.dist-info/RECORD,,
+pmdsky_debug_py-7.0.7.dist-info/METADATA,sha256=ONV-QwwYsGtXyTwabxMyAY0s5IbkX8BIOySH4f_IZc8,1320
+pmdsky_debug_py-7.0.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pmdsky_debug_py-7.0.7.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
+pmdsky_debug_py-7.0.7.dist-info/RECORD,,
```

