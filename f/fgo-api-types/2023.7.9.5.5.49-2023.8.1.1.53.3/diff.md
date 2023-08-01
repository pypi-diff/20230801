# Comparing `tmp/fgo_api_types-2023.7.9.5.5.49.tar.gz` & `tmp/fgo_api_types-2023.8.1.1.53.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.7.9.5.5.49.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.8.1.1.53.3.tar", max compression
```

## Comparing `fgo_api_types-2023.7.9.5.5.49.tar` & `fgo_api_types-2023.8.1.1.53.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-07-09 05:05:22.886548 fgo_api_types-2023.7.9.5.5.49/LICENSE
--rw-r--r--   0        0        0      449 2023-07-09 05:05:22.886548 fgo_api_types-2023.7.9.5.5.49/README.md
--rw-r--r--   0        0        0        0 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/enums.py
--rw-r--r--   0        0        0   160313 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    78686 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/nice.py
--rw-r--r--   0        0        0    53238 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4207 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19183 2023-07-09 05:05:49.418682 fgo_api_types-2023.7.9.5.5.49/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-07-09 05:05:49.882686 fgo_api_types-2023.7.9.5.5.49/pyproject.toml
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.9.5.5.49/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-01 01:52:40.166273 fgo_api_types-2023.8.1.1.53.3/LICENSE
+-rw-r--r--   0        0        0      449 2023-08-01 01:52:40.166273 fgo_api_types-2023.8.1.1.53.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 01:53:03.914244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3738 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38163 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   160790 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    79146 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    53437 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4207 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19183 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-08-01 01:53:04.250244 fgo_api_types-2023.8.1.1.53.3/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.8.1.1.53.3/PKG-INFO
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/LICENSE` & `fgo_api_types-2023.8.1.1.53.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/basic.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/common.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,16 @@
     checkIndvType: Optional[int] = None
     CheckOpponentBuffTypes: Optional[list[NiceBuffType]] = None
     relationId: Optional[NiceBuffRelationOverwrite] = None
     ReleaseText: Optional[str] = None
     DamageRelease: Optional[int] = None
     INDIVIDUALITIE: Optional[NiceTrait] = None
     INDIVIDUALITIE_COUNT_ABOVE: int | None = None
+    INDIVIDUALITIE_AND: list[NiceTrait] | None = None
+    INDIVIDUALITIE_OR: list[NiceTrait] | None = None
     UpBuffRateBuffIndiv: Optional[list[NiceTrait]] = None
     HP_LOWER: Optional[int] = None
     HP_HIGHER: int | None = None
     CounterMessage: str | None = None
     avoidanceText: str | None = None
     gutsText: str | None = None
     missText: str | None = None
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/enums.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,16 @@
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
     # 1000: SvtClass.OTHER,
     # For Support List
     1001: SvtClass.ALL,
     # 1002: SvtClass.EXTRA,
     # 1003: SvtClass.MIX,
+    # 1004: SvtClass.EXTRA1,
+    # 1005: SvtClass.EXTRA2,
 }
 
 
 CLASS_NAME_REVERSE: dict[SvtClass, int] = {v: k for k, v in CLASS_NAME.items()}
 
 
 PLAYABLE_CLASS_LIST = [
@@ -958,14 +960,15 @@
     classBeastILost = "classBeastILost"
     holdingHolyGrail = "holdingHolyGrail"
     standardClassServant = "standardClassServant"
     classBeast = "classBeast"
     classBeastVI = "classBeastVI"
     classBeastVIBoss = "classBeastVIBoss"
     buffBound = "buffBound"
+    buffDamageCut = "buffDamageCut"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -1200,14 +1203,15 @@
     3063: Trait.buffNegativeEffectAtTurnEnd,
     3064: Trait.buffSpecialInvincible,
     3065: Trait.buffSkillRankUp,
     3066: Trait.buffSleep,
     3068: Trait.chenGongNp,
     3070: Trait.buffNullifyBuff,
     3076: Trait.cantBeSacrificed,
+    3085: Trait.buffDamageCut,
     3086: Trait.gutsBlock,
     3087: Trait.buffBound,
     # 6016: No detail
     # 6021: No detail
     # 6022: No detail
     # 10xxx: CCC Kiara buff
     4001: Trait.cardArts,
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/gameenums.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1578,15 +1578,21 @@
     CopyTargetBuffType = 126
     NotSkillCopyTargetFuncIds = 127
     NotSkillCopyTargetIndividualities = 128
     ClassIconAuraEffectId = 129
     ActMasterGenderType = 130
     IntervalTurn = 131
     IntervalCount = 132
-    TargetEnemyRange = 133
+    TriggeredFieldCountTarget = 133
+    TriggeredFieldCountRange = 134
+    TargetEnemyRange = 135
+    TriggeredFuncPositionSameTarget = 136
+    TriggeredFuncPositionAll = 137
+    TriggeredTargetHpRange = 138
+    TriggeredTargetHpRateRange = 139
 
 
 class ClassRelationOverwriteType(IntEnum):
     OVERWRITE_FORCE = 0
     OVERWRITE_MORE_THAN_TARGET = 1
     OVERWRITE_LESS_THAN_TARGET = 2
 
@@ -2188,14 +2194,15 @@
     SVT_SKILL_LV_CLASS_NUM_ABOVE = 180
     SVT_CLASS_LV_UP_COUNT = 181
     SVT_CLASS_SKILL_LV_UP_COUNT = 182
     SVT_CLASS_LIMIT_UP_COUNT = 183
     SVT_CLASS_FRIENDSHIP_COUNT = 184
     COMPLETE_HEEL_PORTRAIT = 185
     NOT_COMPLETE_HEEL_PORTRAIT = 186
+    CLASS_BOARD_SQUARE_RELEASED = 187
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
     questClear = "questClear"
@@ -2377,14 +2384,15 @@
     svtSkillLvClassNumAbove = "svtSkillLvClassNumAbove"
     svtClassLvUpCount = "svtClassLvUpCount"
     svtClassSkillLvUpCount = "svtClassSkillLvUpCount"
     svtClassLimitUpCount = "svtClassLimitUpCount"
     svtClassFriendshipCount = "svtClassFriendshipCount"
     completeHeelPortrait = "completeHeelPortrait"
     notCompleteHeelPortrait = "notCompleteHeelPortrait"
+    classBoardSquareReleased = "classBoardSquareReleased"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
     3: NiceCondType.useItemEternity,
@@ -2564,14 +2572,15 @@
     180: NiceCondType.svtSkillLvClassNumAbove,
     181: NiceCondType.svtClassLvUpCount,
     182: NiceCondType.svtClassSkillLvUpCount,
     183: NiceCondType.svtClassLimitUpCount,
     184: NiceCondType.svtClassFriendshipCount,
     185: NiceCondType.completeHeelPortrait,
     186: NiceCondType.notCompleteHeelPortrait,
+    187: NiceCondType.classBoardSquareReleased,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
     FRIENDSHIP = 3
@@ -4998,14 +5007,15 @@
     NO_DISPLAY_BONUS_ICON = 8
     APPLY_SVT_CHANGE = 16
     HIDE_EQUIP = 32
     NO_DISPLAY_BONUS_ICON_EQUIP = 64
     HIDE_TREASURE_DEVICE_LV = 256
     HIDE_TREASURE_DEVICE_DETAIL = 512
     HIDE_RARITY = 1024
+    NOT_CLASS_BOARD = 2048
 
 
 class NiceNpcServantFollowerFlag(StrEnum):
     """NPC Servant Follower Flag"""
 
     npc = "npc"
     hideSupport = "hideSupport"
@@ -5013,27 +5023,29 @@
     noDisplayBonusIcon = "noDisplayBonusIcon"
     applySvtChange = "applySvtChange"
     hideEquip = "hideEquip"
     noDisplayBonusIconEquip = "noDisplayBonusIconEquip"
     hideTreasureDeviceLv = "hideTreasureDeviceLv"
     hideTreasureDeviceDetail = "hideTreasureDeviceDetail"
     hideRarity = "hideRarity"
+    notClassBoard = "notClassBoard"
 
 
 NPC_SERVANT_FOLLOWER_FLAG_NAME: dict[int, NiceNpcServantFollowerFlag] = {
     1: NiceNpcServantFollowerFlag.npc,
     2: NiceNpcServantFollowerFlag.hideSupport,
     4: NiceNpcServantFollowerFlag.notUsedTreasureDevice,
     8: NiceNpcServantFollowerFlag.noDisplayBonusIcon,
     16: NiceNpcServantFollowerFlag.applySvtChange,
     32: NiceNpcServantFollowerFlag.hideEquip,
     64: NiceNpcServantFollowerFlag.noDisplayBonusIconEquip,
     256: NiceNpcServantFollowerFlag.hideTreasureDeviceLv,
     512: NiceNpcServantFollowerFlag.hideTreasureDeviceDetail,
     1024: NiceNpcServantFollowerFlag.hideRarity,
+    2048: NiceNpcServantFollowerFlag.notClassBoard,
 }
 
 
 class ClassBoardSquareFlag(IntEnum):
     START = 1
     BLANK = 2
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/nice.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,21 @@
     CopyTargetBuffType: list[int] | None = None
     NotSkillCopyTargetFuncIds: list[int] | None = None
     NotSkillCopyTargetIndividualities: list[int] | None = None
     ClassIconAuraEffectId: int | None = None
     ActMasterGenderType: int | None = None
     IntervalTurn: int | None = None
     IntervalCount: int | None = None
+    TriggeredFieldCountTarget: int | None = None
+    TriggeredFieldCountRange: list[int] | None = None
     TargetEnemyRange: list[int] | None = None
+    TriggeredFuncPositionSameTarget: int | None = None
+    TriggeredFuncPositionAll: int | None = None
+    TriggeredTargetHpRange: str | None = None
+    TriggeredTargetHpRateRange: str | None = None
     # Extra dataval from SkillLvEntty.DIC_KEY_APPLY_SUPPORT_SVT
     ApplySupportSvt: Optional[int] = None
     # These are not DataVals but guesses from SkillLvEntity and EventDropUpValInfo
     Individuality: Optional[int] = None
     EventId: Optional[int] = None
     AddCount: Optional[int] = None
     RateCount: Optional[int] = None
@@ -589,16 +595,17 @@
     HP_VAL_LOWER: Optional[list[int]] = None
     HP_PER_HIGHER: Optional[list[int]] = None
     HP_PER_LOWER: Optional[list[int]] = None
     additionalSkillId: Optional[list[int]] = None
     additionalSkillActorType: Optional[list[int]] = None
     tdTypeChangeIDs: list[int] | None = None
     excludeTdChangeTypes: list[int] | None = None
-    SelectAddInfo: list[NiceSelectAddInfo] | None = None
     actRarity: list[list[int]] | None = None
+    battleStartRemainingTurn: list[int] | None = None
+    SelectAddInfo: list[NiceSelectAddInfo] | None = None
 
 
 class NiceSkillAdd(BaseModelORJson):
     priority: int
     releaseConditions: list[NiceCommonRelease]
     name: str
     originalName: str
@@ -1587,23 +1594,26 @@
     )
     targetIds: list[int]
     vals: list[int]
     priority: int
     closedMessage: str
 
 
-class NiceBgmEntity(BaseModelORJson):
+class NiceBgm(BaseModelORJson):
     id: int
     name: str
     originalName: str
     fileName: str
+    notReleased: bool
     audioAsset: Optional[HttpUrl] = None
+
+
+class NiceBgmEntity(NiceBgm):
     priority: int
     detail: str
-    notReleased: bool
     shop: Optional[NiceShop] = None
     logo: HttpUrl
     releaseConditions: list[NiceBgmRelease]
 
 
 class NiceEventQuest(BaseModelORJson):
     questId: int
@@ -1999,22 +2009,14 @@
     startedAt: int
     endedAt: int
     closedAt: int
     missions: list[NiceEventMission]
     quests: list[BasicQuest]
 
 
-class NiceBgm(BaseModelORJson):
-    id: int
-    name: str
-    fileName: str
-    notReleased: bool
-    audioAsset: Optional[HttpUrl] = None
-
-
 class NiceQuestRelease(BaseModelORJson):
     type: NiceCondType
     targetId: int
     value: int
     closedMessage: str
 
 
@@ -2666,7 +2668,18 @@
     closedMessage: str
     condType: NiceCondType
     condTargetId: int
     condNum: int
     classes: list[NiceClassBoardClass]
     squares: list[NiceClassBoardSquare]
     lines: list[NiceClassBoardLine]
+
+
+class NiceFuncTypeDetail(BaseModelORJson):
+    funcType: NiceFuncType
+    ignoreValueUp: bool
+
+
+class NiceBuffTypeDetail(BaseModelORJson):
+    buffType: NiceBuffType
+    ignoreValueUp: bool
+    script: dict[str, Any]
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/raw.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -2170,14 +2170,25 @@
 
 class MstFuncDisp(BaseModelORJson):
     funcIds: list[int]
     id: int
     detail: str
 
 
+class MstFuncTypeDetail(BaseModelORJson):
+    funcType: int
+    ignoreValueUp: bool
+
+
+class MstBuffTypeDetail(BaseModelORJson):
+    buffType: int
+    ignoreValueUp: bool
+    script: dict[str, Any]
+
+
 class ClassBoardEntity(BaseModelORJson):
     mstClassBoardBase: MstClassBoardBase
     mstClassBoardClass: list[MstClassBoardClass]
     mstClassBoardLine: list[MstClassBoardLine]
     mstClassBoardSquare: list[MstClassBoardSquare]
     mstClassBoardLock: list[MstClassBoardLock]
     mstClassBoardCommandSpell: list[MstClassBoardCommandSpell]
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/rayshift.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.9.5.5.49/fgo_api_types/search.py` & `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.7.9.5.5.49/pyproject.toml` & `fgo_api_types-2023.8.1.1.53.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.07.09.05.05.49"
+version = "2023.08.01.01.53.03"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.7.9.5.5.49/PKG-INFO` & `fgo_api_types-2023.8.1.1.53.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.7.9.5.5.49
+Version: 2023.8.1.1.53.3
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

