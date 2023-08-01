# Comparing `tmp/posuto-2023.7.0.tar.gz` & `tmp/posuto-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posuto-2023.7.0.tar", last modified: Sat Jul  1 08:00:07 2023, max compression
+gzip compressed data, was "posuto-2023.8.0.tar", last modified: Tue Aug  1 13:06:09 2023, max compression
```

## Comparing `posuto-2023.7.0.tar` & `posuto-2023.8.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.874369 posuto-2023.7.0/
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.814399 posuto-2023.7.0/.github/
--rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.7.0/.github/FUNDING.yml
--rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.7.0/.gitignore
--rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.7.0/LICENSE
--rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.7.0/MANIFEST.in
--rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.7.0/Makefile
--rw-r--r--   0 23        (1000) u23       (1000)     6435 2023-07-01 08:00:07.874369 posuto-2023.7.0/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.7.0/README.md
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.814399 posuto-2023.7.0/examples/
--rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.7.0/examples/sample.py
--rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.7.0/postcharacter.png
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.874369 posuto-2023.7.0/posuto/
--rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.7.0/posuto/__init__.py
--rw-r--r--   0 23        (1000) u23       (1000) 13069151 2023-07-01 07:57:12.000000 posuto-2023.7.0/posuto/officedata.json
--rw-r--r--   0 23        (1000) u23       (1000) 83795968 2023-07-01 07:57:14.000000 posuto-2023.7.0/posuto/postaldata.db
--rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.7.0/posuto/posuto.py
--rw-r--r--   0 23        (1000) u23       (1000)    11314 2023-06-08 11:14:31.000000 posuto-2023.7.0/posuto/prep.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.874369 posuto-2023.7.0/posuto/tests/
--rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.7.0/posuto/tests/test_basic.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-07-01 08:00:07.874369 posuto-2023.7.0/posuto.egg-info/
--rw-r--r--   0 23        (1000) u23       (1000)     6435 2023-07-01 08:00:07.000000 posuto-2023.7.0/posuto.egg-info/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)      367 2023-07-01 08:00:07.000000 posuto-2023.7.0/posuto.egg-info/SOURCES.txt
--rw-r--r--   0 23        (1000) u23       (1000)        1 2023-07-01 08:00:07.000000 posuto-2023.7.0/posuto.egg-info/dependency_links.txt
--rw-r--r--   0 23        (1000) u23       (1000)        7 2023-07-01 08:00:07.000000 posuto-2023.7.0/posuto.egg-info/top_level.txt
--rw-r--r--   0 23        (1000) u23       (1000)      706 2023-07-01 08:00:07.877701 posuto-2023.7.0/setup.cfg
--rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.7.0/setup.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.877658 posuto-2023.8.0/
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.797657 posuto-2023.8.0/.github/
+-rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.8.0/.github/FUNDING.yml
+-rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.8.0/.gitignore
+-rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.8.0/LICENSE
+-rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.8.0/MANIFEST.in
+-rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.8.0/Makefile
+-rw-r--r--   0 23        (1000) u23       (1000)     6613 2023-08-01 13:06:09.877658 posuto-2023.8.0/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)     5817 2023-07-01 12:46:04.000000 posuto-2023.8.0/README.md
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.797657 posuto-2023.8.0/examples/
+-rw-r--r--   0 23        (1000) u23       (1000)      220 2023-07-01 12:45:10.000000 posuto-2023.8.0/examples/sample.py
+-rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.8.0/postcharacter.png
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.874324 posuto-2023.8.0/posuto/
+-rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.8.0/posuto/__init__.py
+-rw-r--r--   0 23        (1000) u23       (1000) 13065744 2023-08-01 13:03:27.000000 posuto-2023.8.0/posuto/officedata.json
+-rw-r--r--   0 23        (1000) u23       (1000) 83836928 2023-08-01 13:03:29.000000 posuto-2023.8.0/posuto/postaldata.db
+-rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.8.0/posuto/posuto.py
+-rw-r--r--   0 23        (1000) u23       (1000)    11314 2023-06-08 11:14:31.000000 posuto-2023.8.0/posuto/prep.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.877658 posuto-2023.8.0/posuto/tests/
+-rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.8.0/posuto/tests/test_basic.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-08-01 13:06:09.877658 posuto-2023.8.0/posuto.egg-info/
+-rw-r--r--   0 23        (1000) u23       (1000)     6613 2023-08-01 13:06:09.000000 posuto-2023.8.0/posuto.egg-info/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)      388 2023-08-01 13:06:09.000000 posuto-2023.8.0/posuto.egg-info/SOURCES.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        1 2023-08-01 13:06:09.000000 posuto-2023.8.0/posuto.egg-info/dependency_links.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        7 2023-08-01 13:06:09.000000 posuto-2023.8.0/posuto.egg-info/top_level.txt
+-rw-r--r--   0 23        (1000) u23       (1000)       80 2023-07-01 08:00:37.000000 posuto-2023.8.0/requirements-dev.txt
+-rw-r--r--   0 23        (1000) u23       (1000)      706 2023-08-01 13:06:09.877658 posuto-2023.8.0/setup.cfg
+-rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.8.0/setup.py
```

### Comparing `posuto-2023.7.0/.gitignore` & `posuto-2023.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/LICENSE` & `posuto-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/Makefile` & `posuto-2023.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/PKG-INFO` & `posuto-2023.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -37,17 +37,19 @@
 <img src="https://github.com/polm/posuto/raw/master/postcharacter.png" width=125 height=125 alt="Postbox character by Irasutoya" />
 
 Features:
 
 - multi-line neighborhoods are joined
 - parenthetical notes are put in a separate field
 - change reasons are converted from flags to labels
-- romaji and kana records are unified for easy access
+- kana records are unified for easy access
 - codes with multiple areas provide a list of alternates
 
+Romaji provided by JP Post were previously included in this library, but they are extremely low quality and hard to sync, due to being updated separately. If you need romaji it is recommended you use [cutlet](https://github.com/polm/cutlet) instead.
+
 To install:
 
     pip install posuto
 
 Example usage:
 
     import posuto as 〒
@@ -56,16 +58,14 @@
 
     print(🗼)
     # "東京都港区芝公園"
     print(🗼.prefecture)
     # "東京都"
     print(🗼.kana)
     # "トウキョウトミナトクシバコウエン"
-    print(🗼.romaji)
-    # "Tokyo To, Minato Ku, Shibakoen"
     print(🗼.note)
     # None
 
 **Note:** Unfortunately 〒 and 🗼 are not valid identifiers in Python, so the
 above is pseudocode. See [examples/sample.py][] for an executable version.
 
 [examples/sample.py]: https://github.com/polm/posuto/blob/master/examples/sample.py
```

### Comparing `posuto-2023.7.0/README.md` & `posuto-2023.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 <img src="https://github.com/polm/posuto/raw/master/postcharacter.png" width=125 height=125 alt="Postbox character by Irasutoya" />
 
 Features:
 
 - multi-line neighborhoods are joined
 - parenthetical notes are put in a separate field
 - change reasons are converted from flags to labels
-- romaji and kana records are unified for easy access
+- kana records are unified for easy access
 - codes with multiple areas provide a list of alternates
 
+Romaji provided by JP Post were previously included in this library, but they are extremely low quality and hard to sync, due to being updated separately. If you need romaji it is recommended you use [cutlet](https://github.com/polm/cutlet) instead.
+
 To install:
 
     pip install posuto
 
 Example usage:
 
     import posuto as 〒
@@ -34,16 +36,14 @@
 
     print(🗼)
     # "東京都港区芝公園"
     print(🗼.prefecture)
     # "東京都"
     print(🗼.kana)
     # "トウキョウトミナトクシバコウエン"
-    print(🗼.romaji)
-    # "Tokyo To, Minato Ku, Shibakoen"
     print(🗼.note)
     # None
 
 **Note:** Unfortunately 〒 and 🗼 are not valid identifiers in Python, so the
 above is pseudocode. See [examples/sample.py][] for an executable version.
 
 [examples/sample.py]: https://github.com/polm/posuto/blob/master/examples/sample.py
```

### Comparing `posuto-2023.7.0/postcharacter.png` & `posuto-2023.8.0/postcharacter.png`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/posuto/officedata.json` & `posuto-2023.8.0/posuto/officedata.json`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
     "neighborhood": "北一条西",
     "banchi": "5丁目2番地北1条三井ビルディング5F",
     "postal_code": "0608529",
     "old_code": "060  ",
     "post_office": "札幌中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシチュウオウク",
     "neighborhood_kana": "キタ１ジョウニシ",
     "alternates": []
   },
   "0608580": {
     "jis": "01101",
@@ -1848,25 +1848,25 @@
   },
   "0608678": {
     "jis": "01101",
     "kana": "ニホンセイメイホケン ソウゴガイシヤ サツポロシシヤ",
     "name": "日本生命保険　相互会社　札幌支社",
     "prefecture": "北海道",
     "city": "札幌市中央区",
-    "neighborhood": "北四条西",
-    "banchi": "5丁目1番3号(札幌中央郵便局私書箱第126号)",
+    "neighborhood": "北三条西",
+    "banchi": "4丁目1-1(札幌中央郵便局私書箱第126号)",
     "postal_code": "0608678",
     "old_code": "060  ",
     "post_office": "札幌中央",
     "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシチュウオウク",
-    "neighborhood_kana": "キタ４ジョウニシ",
+    "neighborhood_kana": "キタ３ジョウニシ",
     "alternates": []
   },
   "0608616": {
     "jis": "01101",
     "kana": "ニホンロウドウクミアイ ソウレンゴウカイ ホツカイドウレンゴウカイ",
     "name": "日本労働組合　総連合会　北海道連合会",
     "prefecture": "北海道",
@@ -4597,14 +4597,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "サッポロシヒガシク",
     "neighborhood_kana": "ヒガシナエボ２ジョウ",
     "alternates": []
   },
+  "0078511": {
+    "jis": "01103",
+    "kana": "サツラクノウギヨウキヨウドウクミアイ シニユウジギヨウブ",
+    "name": "サツラク農業協同組合　市乳事業部",
+    "prefecture": "北海道",
+    "city": "札幌市東区",
+    "neighborhood": "丘珠町",
+    "banchi": "573-27",
+    "postal_code": "0078511",
+    "old_code": "007  ",
+    "post_office": "丘珠",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ホッカイドウ",
+    "city_kana": "サッポロシヒガシク",
+    "neighborhood_kana": "オカダマチョウ",
+    "alternates": []
+  },
   "0078508": {
     "jis": "01103",
     "kana": "センシユウデンギヨウ カブシキカイシヤ サツポロシテン",
     "name": "泉州電業　株式会社　札幌支店",
     "prefecture": "北海道",
     "city": "札幌市東区",
     "neighborhood": "東苗穂三条",
@@ -15213,15 +15232,15 @@
     "neighborhood": "栄",
     "banchi": "1丁目4番1号",
     "postal_code": "0978678",
     "old_code": "097  ",
     "post_office": "稚内",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ホッカイドウ",
     "city_kana": "ワッカナイシ",
     "neighborhood_kana": "サカエ",
     "alternates": []
   },
   "0978527": {
     "jis": "01214",
@@ -43831,15 +43850,15 @@
     "neighborhood": "金沢",
     "banchi": "720番地の1",
     "postal_code": "9968585",
     "old_code": "996  ",
     "post_office": "新庄",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヤマガタケン",
     "city_kana": "シンジョウシ",
     "neighborhood_kana": "カナザワ",
     "alternates": []
   },
   "9968602": {
     "jis": "06205",
@@ -53980,34 +53999,72 @@
     "neighborhood": "藤本",
     "banchi": "2-1",
     "postal_code": "3058605",
     "old_code": "305  ",
     "post_office": "筑波学園",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "ツクバシ",
     "neighborhood_kana": "フジモト",
     "alternates": []
   },
+  "3058602": {
+    "jis": "08220",
+    "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ キバンギジユツケンキユウホンブイデンシゲンケンキユウセンタ-",
+    "name": "国立研究開発法人　農業・食品産業技術総合研究機構　基盤技術研究本部遺伝資源研究センター",
+    "prefecture": "茨城県",
+    "city": "つくば市",
+    "neighborhood": "観音台",
+    "banchi": "2丁目1-2",
+    "postal_code": "3058602",
+    "old_code": "305  ",
+    "post_office": "筑波学園",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イバラキケン",
+    "city_kana": "ツクバシ",
+    "neighborhood_kana": "カンノンダイ",
+    "alternates": []
+  },
   "3058518": {
     "jis": "08220",
-    "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ジセダイサクモツカイハツケンキユウセンタ-",
-    "name": "国立研究開発法人　農業・食品産業技術総合研究機構　次世代作物開発研究センター",
+    "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ サクモツケンキユウブモン",
+    "name": "国立研究開発法人　農業・食品産業技術総合研究機構　作物研究部門",
     "prefecture": "茨城県",
     "city": "つくば市",
     "neighborhood": "観音台",
-    "banchi": "2-1-2",
+    "banchi": "2丁目1-2",
     "postal_code": "3058518",
     "old_code": "305  ",
     "post_office": "筑波学園",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
+    "prefecture_kana": "イバラキケン",
+    "city_kana": "ツクバシ",
+    "neighborhood_kana": "カンノンダイ",
+    "alternates": []
+  },
+  "3058642": {
+    "jis": "08220",
+    "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ シヨクヒンケンキユウブモン",
+    "name": "国立研究開発法人　農業・食品産業技術総合研究機構　食品研究部門",
+    "prefecture": "茨城県",
+    "city": "つくば市",
+    "neighborhood": "観音台",
+    "banchi": "2丁目1-12",
+    "postal_code": "3058642",
+    "old_code": "305  ",
+    "post_office": "筑波学園",
+    "type": "office",
+    "multiple": false,
+    "new": true,
     "prefecture_kana": "イバラキケン",
     "city_kana": "ツクバシ",
     "neighborhood_kana": "カンノンダイ",
     "alternates": []
   },
   "3058634": {
     "jis": "08220",
@@ -54018,15 +54075,15 @@
     "neighborhood": "大わし",
     "banchi": "1-2",
     "postal_code": "3058634",
     "old_code": "305  ",
     "post_office": "筑波学園",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "ツクバシ",
     "neighborhood_kana": "オオワシ",
     "alternates": []
   },
   "3058666": {
     "jis": "08220",
@@ -54062,14 +54119,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "ツクバシ",
     "neighborhood_kana": "カンノンダイ",
     "alternates": []
   },
+  "3058609": {
+    "jis": "08220",
+    "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ノウソンコウガクケンキユウブモン",
+    "name": "国立研究開発法人　農業・食品産業技術総合研究機構　農村工学研究部門",
+    "prefecture": "茨城県",
+    "city": "つくば市",
+    "neighborhood": "観音台",
+    "banchi": "2丁目1-6",
+    "postal_code": "3058609",
+    "old_code": "305  ",
+    "post_office": "筑波学園",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イバラキケン",
+    "city_kana": "ツクバシ",
+    "neighborhood_kana": "カンノンダイ",
+    "alternates": []
+  },
   "3058519": {
     "jis": "08220",
     "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ヤサイカキケンキユウブモン",
     "name": "国立研究開発法人　農業・食品産業技術総合研究機構　野菜花き研究部門",
     "prefecture": "茨城県",
     "city": "つくば市",
     "neighborhood": "観音台",
@@ -54366,71 +54442,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イバラキケン",
     "city_kana": "ツクバシ",
     "neighborhood_kana": "オノガワ",
     "alternates": []
   },
-  "3058642": {
-    "jis": "08220",
-    "kana": "ドクリツギヨウセイホウジン シヨクヒンソウゴウケンキユウジヨ",
-    "name": "独立行政法人　食品総合研究所",
-    "prefecture": "茨城県",
-    "city": "つくば市",
-    "neighborhood": "観音台",
-    "banchi": "2丁目1-2(筑波農林研究団地内郵便局私書箱第11号)",
-    "postal_code": "3058642",
-    "old_code": "305  ",
-    "post_office": "筑波学園",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イバラキケン",
-    "city_kana": "ツクバシ",
-    "neighborhood_kana": "カンノンダイ",
-    "alternates": []
-  },
-  "3058609": {
-    "jis": "08220",
-    "kana": "ドクリツギヨウセイホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ノウソンコウガクケンキユウシヨ",
-    "name": "独立行政法人　農業・食品産業技術総合研究機構　農村工学研究所",
-    "prefecture": "茨城県",
-    "city": "つくば市",
-    "neighborhood": "観音台",
-    "banchi": "2丁目1-6",
-    "postal_code": "3058609",
-    "old_code": "305  ",
-    "post_office": "筑波学園",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イバラキケン",
-    "city_kana": "ツクバシ",
-    "neighborhood_kana": "カンノンダイ",
-    "alternates": []
-  },
-  "3058602": {
-    "jis": "08220",
-    "kana": "ドクリツギヨウセイホウジン ノウギヨウセイブツシゲンケンキユウジヨ",
-    "name": "独立行政法人　農業生物資源研究所",
-    "prefecture": "茨城県",
-    "city": "つくば市",
-    "neighborhood": "観音台",
-    "banchi": "2丁目1-2(筑波農林研究団地内郵便局私書箱第12号)",
-    "postal_code": "3058602",
-    "old_code": "305  ",
-    "post_office": "筑波学園",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イバラキケン",
-    "city_kana": "ツクバシ",
-    "neighborhood_kana": "カンノンダイ",
-    "alternates": []
-  },
   "3058501": {
     "jis": "08220",
     "kana": "ニホンデンキ カブシキガイシヤ ツクバケンキユウジヨ",
     "name": "日本電気　株式会社　筑波研究所",
     "prefecture": "茨城県",
     "city": "つくば市",
     "neighborhood": "御幸が丘",
@@ -67396,15 +67415,15 @@
     "neighborhood": "桜木町",
     "banchi": "1-195-1大宮ソラミチKOZ8階",
     "postal_code": "3308564",
     "old_code": "330  ",
     "post_office": "さいたま新都心",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "サイタマケン",
     "city_kana": "サイタマシオオミヤク",
     "neighborhood_kana": "サクラギチョウ",
     "alternates": []
   },
   "3309520": {
     "jis": "11103",
@@ -74129,14 +74148,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "サイタマケン",
     "city_kana": "サヤマシ",
     "neighborhood_kana": "ヒロセダイ",
     "alternates": []
   },
+  "3501383": {
+    "jis": "11215",
+    "kana": "アマゾンサヤマヒロセダイエフシ-",
+    "name": "アマゾン狭山広瀬台ＦＣ",
+    "prefecture": "埼玉県",
+    "city": "狭山市",
+    "neighborhood": "広瀬台",
+    "banchi": "2丁目4-3",
+    "postal_code": "3501383",
+    "old_code": "35013",
+    "post_office": "狭山",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "サイタマケン",
+    "city_kana": "サヤマシ",
+    "neighborhood_kana": "ヒロセダイ",
+    "alternates": []
+  },
   "3501395": {
     "jis": "11215",
     "kana": "カブシキガイシヤ サギノミヤセイサクシヨ サヤマジギヨウシヨ",
     "name": "株式会社　鷺宮製作所　狭山事業所",
     "prefecture": "埼玉県",
     "city": "狭山市",
     "neighborhood": "笹井",
@@ -77277,15 +77315,15 @@
     "neighborhood": "菖蒲町三箇",
     "banchi": "5番5",
     "postal_code": "3460181",
     "old_code": "34601",
     "post_office": "久喜",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "サイタマケン",
     "city_kana": "クキシ",
     "neighborhood_kana": "ショウブチョウサンガ",
     "alternates": []
   },
   "3460198": {
     "jis": "11232",
@@ -82693,15 +82731,15 @@
     "neighborhood": "新港",
     "banchi": "68-1",
     "postal_code": "2618528",
     "old_code": "261  ",
     "post_office": "美浜",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "チバシミハマク",
     "neighborhood_kana": "シンミナト",
     "alternates": []
   },
   "2618515": {
     "jis": "12106",
@@ -90104,15 +90142,15 @@
     "neighborhood": "舞浜",
     "banchi": "1番地2",
     "postal_code": "2798526",
     "old_code": "279  ",
     "post_office": "浦安",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "チバケン",
     "city_kana": "ウラヤスシ",
     "neighborhood_kana": "マイハマ",
     "alternates": []
   },
   "2798519": {
     "jis": "12227",
@@ -91312,26 +91350,26 @@
     "prefecture_kana": "チバケン",
     "city_kana": "カトリシ",
     "neighborhood_kana": "ニラ",
     "alternates": []
   },
   "2891297": {
     "jis": "12237",
-    "kana": "アルバツクマテリアル カブシキガイシヤ",
-    "name": "アルバックマテリアル　株式会社",
+    "kana": "カブシキガイシヤ アルバツク",
+    "name": "株式会社　アルバック",
     "prefecture": "千葉県",
     "city": "山武市",
     "neighborhood": "横田",
     "banchi": "516番地",
     "postal_code": "2891297",
     "old_code": "28912",
     "post_office": "日向",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "チバケン",
     "city_kana": "サンムシ",
     "neighborhood_kana": "ヨコタ",
     "alternates": []
   },
   "2891298": {
     "jis": "12237",
@@ -97869,33 +97907,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "ソトカンダ",
     "alternates": []
   },
-  "1018476": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ キツズステ-シヨン",
-    "name": "（株）　キッズステーション",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田錦町",
-    "banchi": "3丁目26一ツ橋SIビル10階",
-    "postal_code": "1018476",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダニシキチョウ",
-    "alternates": []
-  },
   "1018589": {
     "jis": "13101",
     "kana": "カブシキガイシヤ キヨクトウシヨウカイ/カブシキガイシヤ カパス",
     "name": "株式会社　極東商会／株式会社　カパス",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "外神田",
@@ -98439,33 +98458,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダヒガシマツシタチョウ",
     "alternates": []
   },
-  "1018901": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ニホンマンパワ-ナイ カンポエルシ-ジムキヨク",
-    "name": "株式会社　日本マンパワー内かんぽＬＣ事務局",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田東松下町",
-    "banchi": "47-1",
-    "postal_code": "1018901",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダヒガシマツシタチョウ",
-    "alternates": []
-  },
   "1018565": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ヒガシニツポンギンコウ カンダシテン",
     "name": "株式会社　東日本銀行　神田支店",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田富山町",
@@ -98610,33 +98610,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダジンボウチョウ",
     "alternates": []
   },
-  "1018972": {
-    "jis": "13101",
-    "kana": "カブシキガイシヤ ミツウロコ",
-    "name": "株式会社　ミツウロコ",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "4丁目14-1",
-    "postal_code": "1018972",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018648": {
     "jis": "13101",
     "kana": "カブシキガイシヤ ヤクジニツポウシヤ",
     "name": "株式会社　薬事日報社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田和泉町",
@@ -98864,21 +98845,21 @@
   "1018311": {
     "jis": "13101",
     "kana": "キヨウリンセイヤク カブシキガイシヤ",
     "name": "杏林製薬　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
-    "banchi": "4-6御茶ノ水ソラシティ",
+    "banchi": "4-6",
     "postal_code": "1018311",
     "old_code": "101  ",
     "post_office": "神田",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
   "1018645": {
     "jis": "13101",
@@ -99807,33 +99788,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダイズミチョウ",
     "alternates": []
   },
-  "1018946": {
-    "jis": "13101",
-    "kana": "ニツポンレンタカ-ア-バンネツト カブシキガイシヤ トウキヨウデイビジヨン",
-    "name": "ニッポンレンタカーアーバンネット　株式会社　東京ディビジョン",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "東神田",
-    "banchi": "2丁目1-11第一坂本ビル",
-    "postal_code": "1018946",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ヒガシカンダ",
-    "alternates": []
-  },
   "1018710": {
     "jis": "13101",
     "kana": "ニホンシユツパンハンバイ",
     "name": "日本出版販売　（株）",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田駿河台",
@@ -99997,33 +99959,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018971": {
-    "jis": "13101",
-    "kana": "ヒタチデンセン カブシキガイシヤ",
-    "name": "日立電線　（株）",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "4丁目14-1秋葉原UDX",
-    "postal_code": "1018971",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018439": {
     "jis": "13101",
     "kana": "ヒトツバシダイガク チヨダキヤンパスジムシツ",
     "name": "一橋大学　千代田キャンパス事務室",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "一ツ橋",
@@ -100092,33 +100035,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダミクラチョウ",
     "alternates": []
   },
-  "1018970": {
-    "jis": "13101",
-    "kana": "フルカワスカイ カブシキガイシヤ",
-    "name": "古河スカイ　株式会社",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "外神田",
-    "banchi": "4丁目14-1秋葉原UDX",
-    "postal_code": "1018970",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "ソトカンダ",
-    "alternates": []
-  },
   "1018477": {
     "jis": "13101",
     "kana": "ミズノ カブシキガイシヤ",
     "name": "ミズノ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田小川町",
@@ -100149,14 +100073,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダスルガダイ",
     "alternates": []
   },
+  "1018443": {
+    "jis": "13101",
+    "kana": "ミズホリサ-チアンドテクノロジ-ズ カブシキガイシヤ",
+    "name": "みずほリサーチ＆テクノロジーズ　株式会社",
+    "prefecture": "東京都",
+    "city": "千代田区",
+    "neighborhood": "神田錦町",
+    "banchi": "2丁目3",
+    "postal_code": "1018443",
+    "old_code": "101  ",
+    "post_office": "神田",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "チヨダク",
+    "neighborhood_kana": "カンダニシキチョウ",
+    "alternates": []
+  },
   "1018429": {
     "jis": "13101",
     "kana": "ミタニサンギヨウ カブシキガイシヤ",
     "name": "三谷産業　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田神保町",
@@ -100415,33 +100358,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "カンダニシキチョウ",
     "alternates": []
   },
-  "1018315": {
-    "jis": "13101",
-    "kana": "ロウドウキンコカイカン",
-    "name": "労働金庫会館",
-    "prefecture": "東京都",
-    "city": "千代田区",
-    "neighborhood": "神田駿河台",
-    "banchi": "2丁目5-15",
-    "postal_code": "1018315",
-    "old_code": "101  ",
-    "post_office": "神田",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チヨダク",
-    "neighborhood_kana": "カンダスルガダイ",
-    "alternates": []
-  },
   "1018642": {
     "jis": "13101",
     "kana": "ワイケイケイ カブシキガイシヤ",
     "name": "ＹＫＫ　株式会社",
     "prefecture": "東京都",
     "city": "千代田区",
     "neighborhood": "神田和泉町",
@@ -101663,15 +101587,15 @@
     "neighborhood": "麹町",
     "banchi": "1丁目6番9号DIK麹町ビル703号室",
     "postal_code": "1028301",
     "old_code": "102  ",
     "post_office": "麹町",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チヨダク",
     "neighborhood_kana": "コウジマチ",
     "alternates": []
   },
   "1028622": {
     "jis": "13101",
@@ -108492,33 +108416,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ニホンバシホンチョウ",
     "alternates": []
   },
-  "1038423": {
-    "jis": "13102",
-    "kana": "デイ-エムミツイセイトウ カブシキガイシヤ",
-    "name": "ＤＭ三井製糖　株式会社",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "日本橋箱崎町",
-    "banchi": "36-2Daiwaリバーゲート12階",
-    "postal_code": "1038423",
-    "old_code": "103  ",
-    "post_office": "日本橋",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ニホンバシハコザキチョウ",
-    "alternates": []
-  },
   "1038233": {
     "jis": "13102",
     "kana": "デイアイシ- カブシキガイシヤ",
     "name": "ＤＩＣ　株式会社",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "日本橋",
@@ -111342,52 +111247,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "チュウオウク",
     "neighborhood_kana": "ツキジ",
     "alternates": []
   },
-  "1048572": {
-    "jis": "13102",
-    "kana": "カブシキガイシヤ ピ-エスミツビシ トウキヨウドボク・ケンチクシテン",
-    "name": "株式会社　ピーエス三菱　東京土木・建築支店",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "晴海",
-    "banchi": "2丁目5-24晴海センタービル2階",
-    "postal_code": "1048572",
-    "old_code": "104  ",
-    "post_office": "晴海",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ハルミ",
-    "alternates": []
-  },
-  "1048215": {
-    "jis": "13102",
-    "kana": "カブシキガイシヤ ピ-エスミツビシ ホンシヤ",
-    "name": "株式会社　ピーエス三菱　本社",
-    "prefecture": "東京都",
-    "city": "中央区",
-    "neighborhood": "晴海",
-    "banchi": "2丁目5-24晴海センタービル3階",
-    "postal_code": "1048215",
-    "old_code": "104  ",
-    "post_office": "晴海",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "チュウオウク",
-    "neighborhood_kana": "ハルミ",
-    "alternates": []
-  },
   "1048340": {
     "jis": "13102",
     "kana": "カブシキガイシヤ ブリヂストン",
     "name": "株式会社　ブリヂストン",
     "prefecture": "東京都",
     "city": "中央区",
     "neighborhood": "京橋",
@@ -121581,15 +121448,15 @@
     "neighborhood": "港南",
     "banchi": "1-9-1",
     "postal_code": "1088505",
     "old_code": "108  ",
     "post_office": "高輪",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "コウナン",
     "alternates": []
   },
   "1088220": {
     "jis": "13103",
@@ -124488,15 +124355,15 @@
     "neighborhood": "三田",
     "banchi": "3-5-19住友不動産東京三田ガーデンタワー",
     "postal_code": "1088575",
     "old_code": "108  ",
     "post_office": "高輪",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ミナトク",
     "neighborhood_kana": "ミタ",
     "alternates": []
   },
   "1088388": {
     "jis": "13103",
@@ -125978,33 +125845,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シンジュクク",
     "neighborhood_kana": "シンジュク",
     "alternates": []
   },
-  "1608308": {
-    "jis": "13104",
-    "kana": "クラブツ-リズム カブシキガイシヤ",
-    "name": "クラブツーリズム　株式会社",
-    "prefecture": "東京都",
-    "city": "新宿区",
-    "neighborhood": "西新宿",
-    "banchi": "6丁目3-1新宿アイランドウイング",
-    "postal_code": "1608308",
-    "old_code": "160  ",
-    "post_office": "新宿",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "シンジュクク",
-    "neighborhood_kana": "ニシシンジュク",
-    "alternates": []
-  },
   "1608582": {
     "jis": "13104",
     "kana": "ケイオウギジユクダイガク イガクブ",
     "name": "慶應義塾大学　医学部",
     "prefecture": "東京都",
     "city": "新宿区",
     "neighborhood": "信濃町",
@@ -134666,26 +134514,26 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "ブンキョウク",
     "neighborhood_kana": "ホンゴウ",
     "alternates": []
   },
   "1138663": {
     "jis": "13105",
-    "kana": "ドクリツギヨウセイホウジン ジヨウホウシヨリスイシンキコウ アイテイ-ジンザイイクセイセンタ- コツカシカク・シケンブ",
-    "name": "独立行政法人　情報処理推進機構　ＩＴ人材育成センター　国家資格・試験部",
+    "kana": "ドクリツギヨウセイホウジン ジヨウホウシヨリスイシンキコウ デジタルジンザイセンタ- コツカシカク・シケンブ",
+    "name": "独立行政法人　情報処理推進機構　デジタル人材センター　国家資格・試験部",
     "prefecture": "東京都",
     "city": "文京区",
     "neighborhood": "本駒込",
     "banchi": "2丁目28-8文京グリーンコートセンターオフィス15階",
     "postal_code": "1138663",
     "old_code": "113  ",
     "post_office": "本郷",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ブンキョウク",
     "neighborhood_kana": "ホンコマゴメ",
     "alternates": []
   },
   "1138602": {
     "jis": "13105",
@@ -136539,15 +136387,15 @@
     "neighborhood": "東上野",
     "banchi": "1-7-2",
     "postal_code": "1108646",
     "old_code": "110  ",
     "post_office": "上野",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "タイトウク",
     "neighborhood_kana": "ヒガシウエノ",
     "alternates": []
   },
   "1108722": {
     "jis": "13106",
@@ -141029,14 +140877,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "コウトウク",
     "neighborhood_kana": "トヨス",
     "alternates": []
   },
+  "1358178": {
+    "jis": "13108",
+    "kana": "エヌ・テイ・テイ・デ-タ・カスタマサ-ビス カブシキガイシヤ",
+    "name": "エヌ・ティ・ティ・データ・カスタマサービス　株式会社",
+    "prefecture": "東京都",
+    "city": "江東区",
+    "neighborhood": "豊洲",
+    "banchi": "3-3-9豊洲センタービルアネックス32F",
+    "postal_code": "1358178",
+    "old_code": "135  ",
+    "post_office": "晴海",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "トウキョウト",
+    "city_kana": "コウトウク",
+    "neighborhood_kana": "トヨス",
+    "alternates": []
+  },
   "1358508": {
     "jis": "13108",
     "kana": "オ-ク カブシキガイシヤ",
     "name": "オーク　株式会社",
     "prefecture": "東京都",
     "city": "江東区",
     "neighborhood": "木場",
@@ -147227,33 +147094,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "トウキョウト",
     "city_kana": "シナガワク",
     "neighborhood_kana": "オオサキ",
     "alternates": []
   },
-  "1058711": {
-    "jis": "13109",
-    "kana": "カブシキガイシヤ エツクスワン",
-    "name": "株式会社　エックスワン",
-    "prefecture": "東京都",
-    "city": "品川区",
-    "neighborhood": "大崎",
-    "banchi": "1丁目11-2(芝郵便局私書箱第211号)",
-    "postal_code": "1058711",
-    "old_code": "141  ",
-    "post_office": "芝",
-    "type": "box",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "トウキョウト",
-    "city_kana": "シナガワク",
-    "neighborhood_kana": "オオサキ",
-    "alternates": []
-  },
   "1098792": {
     "jis": "13109",
     "kana": "カブシキガイシヤ カンポセイメイホケン トウキヨウサ-ビスセンタ-",
     "name": "株式会社　かんぽ生命保険　東京サービスセンター",
     "prefecture": "東京都",
     "city": "品川区",
     "neighborhood": "北品川",
@@ -164695,26 +164543,26 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "キタク",
     "neighborhood_kana": "ニシガハラ",
     "alternates": []
   },
   "1148535": {
     "jis": "13117",
-    "kana": "トウキヨウガス ホクブジギヨウホンブ",
-    "name": "東京ガス　（株）　北部事業本部",
+    "kana": "トウキヨウガスネツトワ-ク (カブ)",
+    "name": "東京ガスネットワーク　（株）",
     "prefecture": "東京都",
     "city": "北区",
     "neighborhood": "滝野川",
-    "banchi": "5丁目42",
+    "banchi": "5-42",
     "postal_code": "1148535",
     "old_code": "114  ",
     "post_office": "王子",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "キタク",
     "neighborhood_kana": "タキノガワ",
     "alternates": []
   },
   "1148524": {
     "jis": "13117",
@@ -171896,29 +171744,29 @@
     "prefecture_kana": "トウキョウト",
     "city_kana": "ハチオウジシ",
     "neighborhood_kana": "オカドマチ",
     "alternates": []
   },
   "1928585": {
     "jis": "13201",
-    "kana": "ニホンヒユ-レツト・パツカ-ド カブシキガイシヤ ハチオウジジギヨウシヨ",
-    "name": "日本ヒューレット・パッカード　株式会社　八王子事業所",
+    "kana": "ニホンヒユ-レツト・パツカ-ド ゴウドウカイシヤ",
+    "name": "日本ヒューレット・パッカード　合同会社",
     "prefecture": "東京都",
     "city": "八王子市",
-    "neighborhood": "明神町",
-    "banchi": "4丁目9-8",
+    "neighborhood": "東町",
+    "banchi": "9-8八王子東町センタービル2F",
     "postal_code": "1928585",
     "old_code": "192  ",
     "post_office": "八王子",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "トウキョウト",
     "city_kana": "ハチオウジシ",
-    "neighborhood_kana": "ミョウジンチョウ",
+    "neighborhood_kana": "アズマチョウ",
     "alternates": []
   },
   "1920986": {
     "jis": "13201",
     "kana": "ニホンブンカダイガク",
     "name": "日本文化大學",
     "prefecture": "東京都",
@@ -183675,14 +183523,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "ヨコハマシナカク",
     "neighborhood_kana": "ヤマシタチョウ",
     "alternates": []
   },
+  "2318455": {
+    "jis": "14104",
+    "kana": "ヨコハマシシミンブンカカイカンカンナイホ-ル",
+    "name": "横浜市市民文化会館関内ホール",
+    "prefecture": "神奈川県",
+    "city": "横浜市中区",
+    "neighborhood": "住吉町",
+    "banchi": "4-42-1",
+    "postal_code": "2318455",
+    "old_code": "231  ",
+    "post_office": "横浜港",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "カナガワケン",
+    "city_kana": "ヨコハマシナカク",
+    "neighborhood_kana": "スミヨシチョウ",
+    "alternates": []
+  },
   "2318307": {
     "jis": "14104",
     "kana": "ヨコハマシユウソウセイキユウジムセンタ-",
     "name": "横浜市郵送請求事務センター",
     "prefecture": "神奈川県",
     "city": "横浜市中区",
     "neighborhood": "桜木町",
@@ -191828,33 +191695,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "カナガワケン",
     "city_kana": "サガミハラシミナミク",
     "neighborhood_kana": "キタザト",
     "alternates": []
   },
-  "2520380": {
-    "jis": "14153",
-    "kana": "キタサトダイガクヒガシビヨウイン",
-    "name": "北里大学東病院",
-    "prefecture": "神奈川県",
-    "city": "相模原市南区",
-    "neighborhood": "麻溝台",
-    "banchi": "2丁目1-1",
-    "postal_code": "2520380",
-    "old_code": "228  ",
-    "post_office": "座間",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "カナガワケン",
-    "city_kana": "サガミハラシミナミク",
-    "neighborhood_kana": "アサミゾダイ",
-    "alternates": []
-  },
   "2520375": {
     "jis": "14153",
     "kana": "キタサトダイガクビヨウイン",
     "name": "北里大学病院",
     "prefecture": "神奈川県",
     "city": "相模原市南区",
     "neighborhood": "北里",
@@ -196863,14 +196711,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ニイガタシヒガシク",
     "neighborhood_kana": "タケオオロシシンマチ",
     "alternates": []
   },
+  "9508701": {
+    "jis": "15102",
+    "kana": "クロスウイルメデイカル カブシキガイシヤ",
+    "name": "クロスウィルメディカル　株式会社",
+    "prefecture": "新潟県",
+    "city": "新潟市東区",
+    "neighborhood": "紫竹卸新町",
+    "banchi": "1808番地22",
+    "postal_code": "9508701",
+    "old_code": "950  ",
+    "post_office": "新潟中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ニイガタケン",
+    "city_kana": "ニイガタシヒガシク",
+    "neighborhood_kana": "シチクオロシシンマチ",
+    "alternates": []
+  },
   "9508680": {
     "jis": "15102",
     "kana": "コウリツダイガクホウジン ニイガタケンリツダイガク",
     "name": "公立大学法人　新潟県立大学",
     "prefecture": "新潟県",
     "city": "新潟市東区",
     "neighborhood": "海老ケ瀬",
@@ -202905,14 +202772,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ナガオカシ",
     "neighborhood_kana": "カミイワイ",
     "alternates": []
   },
+  "9402492": {
+    "jis": "15202",
+    "kana": "ナガオカシヤクシヨヨイタシシヨ",
+    "name": "長岡市役所与板支所",
+    "prefecture": "新潟県",
+    "city": "長岡市",
+    "neighborhood": "与板町与板",
+    "banchi": "甲134番地",
+    "postal_code": "9402492",
+    "old_code": "94024",
+    "post_office": "与板",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ニイガタケン",
+    "city_kana": "ナガオカシ",
+    "neighborhood_kana": "ヨイタマチヨイタ",
+    "alternates": []
+  },
   "9402595": {
     "jis": "15202",
     "kana": "カクジヨウギヨルイホ-ルデイングス カブシキガイシヤ",
     "name": "角上魚類ホールディングス　株式会社",
     "prefecture": "新潟県",
     "city": "長岡市",
     "neighborhood": "寺泊",
@@ -202924,14 +202810,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "ニイガタケン",
     "city_kana": "ナガオカシ",
     "neighborhood_kana": "テラドマリ",
     "alternates": []
   },
+  "9402592": {
+    "jis": "15202",
+    "kana": "ナガオカシヤクシヨテラドマリシシヨ",
+    "name": "長岡市役所寺泊支所",
+    "prefecture": "新潟県",
+    "city": "長岡市",
+    "neighborhood": "寺泊",
+    "banchi": "鳥帽子平1977番地8",
+    "postal_code": "9402592",
+    "old_code": "94025",
+    "post_office": "寺泊",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "ニイガタケン",
+    "city_kana": "ナガオカシ",
+    "neighborhood_kana": "テラドマリ",
+    "alternates": []
+  },
   "9495292": {
     "jis": "15202",
     "kana": "ナガオカシヤクシヨ オグニシシヨ",
     "name": "長岡市役所　小国支所",
     "prefecture": "新潟県",
     "city": "長岡市",
     "neighborhood": "小国町法坂",
@@ -220168,33 +220073,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "コマツシ",
     "neighborhood_kana": "クシマチ",
     "alternates": []
   },
-  "9238552": {
-    "jis": "17203",
-    "kana": "セイケイゲカ ロジヨウビヨウイン",
-    "name": "整形外科　芦城病院",
-    "prefecture": "石川県",
-    "city": "小松市",
-    "neighborhood": "大文字町",
-    "banchi": "88",
-    "postal_code": "9238552",
-    "old_code": "923  ",
-    "post_office": "小松",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "イシカワケン",
-    "city_kana": "コマツシ",
-    "neighborhood_kana": "ダイモンジチョウ",
-    "alternates": []
-  },
   "9238581": {
     "jis": "17203",
     "kana": "ダイキヨウ カブシキガイシヤ",
     "name": "大京　株式会社",
     "prefecture": "石川県",
     "city": "小松市",
     "neighborhood": "串町",
@@ -220263,14 +220149,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "イシカワケン",
     "city_kana": "コマツシ",
     "neighborhood_kana": "コクフダイ",
     "alternates": []
   },
+  "9238552": {
+    "jis": "17203",
+    "kana": "トクテイイリヨウホウジンシヤダン カツキカイ ロジヨウクリニツク",
+    "name": "特定医療法人社団　勝木会　芦城クリニック",
+    "prefecture": "石川県",
+    "city": "小松市",
+    "neighborhood": "土居原町",
+    "banchi": "175",
+    "postal_code": "9238552",
+    "old_code": "923  ",
+    "post_office": "小松",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "イシカワケン",
+    "city_kana": "コマツシ",
+    "neighborhood_kana": "ドイハラマチ",
+    "alternates": []
+  },
   "9238633": {
     "jis": "17203",
     "kana": "ニホンデンシンデンワ カブシキガイシヤ コマツシテン",
     "name": "日本電信電話　株式会社　小松支店",
     "prefecture": "石川県",
     "city": "小松市",
     "neighborhood": "末広町",
@@ -226686,50 +226591,50 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクイケン",
     "city_kana": "オオノシ",
     "neighborhood_kana": "アサヒ",
     "alternates": []
   },
-  "9118555": {
+  "9118501": {
     "jis": "18206",
-    "kana": "アボツトジヤパン カブシキガイシヤ カツヤマジギヨウシヨ",
-    "name": "アボットジャパン　株式会社　勝山事業所",
+    "kana": "カツヤマシヤクシヨ",
+    "name": "勝山市役所",
     "prefecture": "福井県",
     "city": "勝山市",
-    "neighborhood": "猪野口",
-    "banchi": "37-1-1(勝山郵便局私書箱第4号)",
-    "postal_code": "9118555",
+    "neighborhood": "元町",
+    "banchi": "1丁目1-1",
+    "postal_code": "9118501",
     "old_code": "911  ",
     "post_office": "勝山",
-    "type": "box",
+    "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "フクイケン",
     "city_kana": "カツヤマシ",
-    "neighborhood_kana": "イノクチ",
+    "neighborhood_kana": "モトマチ",
     "alternates": []
   },
-  "9118501": {
+  "9118555": {
     "jis": "18206",
-    "kana": "カツヤマシヤクシヨ",
-    "name": "勝山市役所",
+    "kana": "カツヤマフア-マ カブシキガイシヤ",
+    "name": "勝山ファーマ　株式会社",
     "prefecture": "福井県",
     "city": "勝山市",
-    "neighborhood": "元町",
-    "banchi": "1丁目1-1",
-    "postal_code": "9118501",
+    "neighborhood": "猪野口",
+    "banchi": "37字2番1号(勝山郵便局私書箱第4号)",
+    "postal_code": "9118555",
     "old_code": "911  ",
     "post_office": "勝山",
-    "type": "office",
+    "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "フクイケン",
     "city_kana": "カツヤマシ",
-    "neighborhood_kana": "モトマチ",
+    "neighborhood_kana": "イノクチ",
     "alternates": []
   },
   "9118585": {
     "jis": "18206",
     "kana": "カブシキガイシヤ イツポンギクボホンテン",
     "name": "株式会社　一本義久保本店",
     "prefecture": "福井県",
@@ -227516,15 +227421,15 @@
     "neighborhood": "妙法寺町",
     "banchi": "29号2",
     "postal_code": "9158577",
     "old_code": "915  ",
     "post_office": "武生",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクイケン",
     "city_kana": "エチゼンシ",
     "neighborhood_kana": "ミョウホウジチョウ",
     "alternates": []
   },
   "9158515": {
     "jis": "18209",
@@ -232590,15 +232495,15 @@
     "neighborhood": "七瀬",
     "banchi": "4-5",
     "postal_code": "3808550",
     "old_code": "380  ",
     "post_office": "長野中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ナガノケン",
     "city_kana": "ナガノシ",
     "neighborhood_kana": "ナナセ",
     "alternates": []
   },
   "3808586": {
     "jis": "20201",
@@ -305679,15 +305584,15 @@
     "neighborhood": "四条通麩屋町西入",
     "banchi": "立売東町28-2大和証券京都ビル2階",
     "postal_code": "6008522",
     "old_code": "600  ",
     "post_office": "京都中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "6008688": {
     "jis": "26106",
@@ -321096,15 +321001,15 @@
     "neighborhood": "松下町",
     "banchi": "1番1号",
     "postal_code": "5708511",
     "old_code": "570  ",
     "post_office": "守口",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オオサカフ",
     "city_kana": "モリグチシ",
     "neighborhood_kana": "マツシタチョウ",
     "alternates": []
   },
   "5708540": {
     "jis": "27209",
@@ -330349,15 +330254,15 @@
     "neighborhood": "上内膳",
     "banchi": "222-1",
     "postal_code": "6568555",
     "old_code": "656  ",
     "post_office": "洲本",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヒョウゴケン",
     "city_kana": "スモトシ",
     "neighborhood_kana": "カミナイゼン",
     "alternates": []
   },
   "6561395": {
     "jis": "28205",
@@ -334043,26 +333948,26 @@
     "prefecture_kana": "ヒョウゴケン",
     "city_kana": "イボグンタイシチョウ",
     "neighborhood_kana": "イカルガ",
     "alternates": []
   },
   "6711592": {
     "jis": "28464",
-    "kana": "タイシチヨウヤクバ",
-    "name": "太子町役場",
+    "kana": "ヒヨウゴケンイボグンタイシチヨウヤクバ",
+    "name": "兵庫県揖保郡太子町役場",
     "prefecture": "兵庫県",
     "city": "揖保郡太子町",
     "neighborhood": "鵤",
-    "banchi": "1369-1(太子郵便局私書箱第6号)",
+    "banchi": "280番地1",
     "postal_code": "6711592",
     "old_code": "67115",
     "post_office": "太子",
-    "type": "box",
+    "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "ヒョウゴケン",
     "city_kana": "イボグンタイシチョウ",
     "neighborhood_kana": "イカルガ",
     "alternates": []
   },
   "6781292": {
     "jis": "28481",
@@ -343997,88 +343902,88 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "ヤスギシ",
     "neighborhood_kana": "カメシマチョウ",
     "alternates": []
   },
-  "6928606": {
+  "6928510": {
     "jis": "32206",
-    "kana": "カブシキガイシヤ ヒタチキンゾクヤスギセイサクシヨ",
-    "name": "株式会社　日立金属安来製作所",
+    "kana": "カブシキガイシヤ フ-ズマ-ケツトホツク",
+    "name": "株式会社　フーズマーケットホック",
     "prefecture": "島根県",
     "city": "安来市",
-    "neighborhood": "飯島町",
-    "banchi": "1240番地5(安来郵便局私書箱第6号)",
-    "postal_code": "6928606",
+    "neighborhood": "赤江町",
+    "banchi": "1448-1",
+    "postal_code": "6928510",
     "old_code": "692  ",
     "post_office": "安来",
-    "type": "box",
+    "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "ヤスギシ",
-    "neighborhood_kana": "ハシマチョウ",
+    "neighborhood_kana": "アカエチョウ",
     "alternates": []
   },
-  "6928510": {
+  "6928601": {
     "jis": "32206",
-    "kana": "カブシキガイシヤ フ-ズマ-ケツトホツク",
-    "name": "株式会社　フーズマーケットホック",
+    "kana": "カブシキガイシヤ プロテリアル ヤスギコウジヨウ",
+    "name": "株式会社　プロテリアル　安来工場",
     "prefecture": "島根県",
     "city": "安来市",
-    "neighborhood": "赤江町",
-    "banchi": "1448-1",
-    "postal_code": "6928510",
+    "neighborhood": "安来町",
+    "banchi": "2107-2(安来郵便局私書箱第1号)",
+    "postal_code": "6928601",
     "old_code": "692  ",
     "post_office": "安来",
-    "type": "office",
+    "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "シマネケン",
     "city_kana": "ヤスギシ",
-    "neighborhood_kana": "アカエチョウ",
+    "neighborhood_kana": "ヤスギチョウ",
     "alternates": []
   },
-  "6928550": {
+  "6928606": {
     "jis": "32206",
-    "kana": "タカバヤシシヨウジ カブシキカイシヤ",
-    "name": "高林商事　株式会社",
+    "kana": "カブシキガイシヤ プロテリアルヤスギセイサクシヨ",
+    "name": "株式会社　プロテリアル安来製作所",
     "prefecture": "島根県",
     "city": "安来市",
-    "neighborhood": "恵乃島町",
-    "banchi": "113-16",
-    "postal_code": "6928550",
+    "neighborhood": "飯島町",
+    "banchi": "1240番地2(安来郵便局私書箱第6号)",
+    "postal_code": "6928606",
     "old_code": "692  ",
     "post_office": "安来",
-    "type": "office",
+    "type": "box",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "シマネケン",
     "city_kana": "ヤスギシ",
-    "neighborhood_kana": "エノシマチョウ",
+    "neighborhood_kana": "ハシマチョウ",
     "alternates": []
   },
-  "6928601": {
+  "6928550": {
     "jis": "32206",
-    "kana": "ヒタチキンゾク カブシキカイシヤ ヤスギコウジヨウ",
-    "name": "日立金属　株式会社　安来工場",
+    "kana": "タカバヤシシヨウジ カブシキカイシヤ",
+    "name": "高林商事　株式会社",
     "prefecture": "島根県",
     "city": "安来市",
-    "neighborhood": "安来町",
-    "banchi": "2107-2(安来郵便局私書箱第1号)",
-    "postal_code": "6928601",
+    "neighborhood": "恵乃島町",
+    "banchi": "113-16",
+    "postal_code": "6928550",
     "old_code": "692  ",
     "post_office": "安来",
-    "type": "box",
+    "type": "office",
     "multiple": false,
     "new": false,
     "prefecture_kana": "シマネケン",
     "city_kana": "ヤスギシ",
-    "neighborhood_kana": "ヤスギチョウ",
+    "neighborhood_kana": "エノシマチョウ",
     "alternates": []
   },
   "6928686": {
     "jis": "32206",
     "kana": "ヤスギシヤクシヨ",
     "name": "安来市役所",
     "prefecture": "島根県",
@@ -345967,15 +345872,15 @@
     "neighborhood": "駅元町",
     "banchi": "6番26号",
     "postal_code": "7008569",
     "old_code": "700  ",
     "post_office": "岡山中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "オカヤマケン",
     "city_kana": "オカヤマシキタク",
     "neighborhood_kana": "エキモトマチ",
     "alternates": []
   },
   "7008522": {
     "jis": "33101",
@@ -364382,15 +364287,15 @@
     "neighborhood": "寿町",
     "banchi": "6番39号防府地方合同庁舎",
     "postal_code": "7478533",
     "old_code": "747  ",
     "post_office": "防府",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "ヤマグチケン",
     "city_kana": "ホウフシ",
     "neighborhood_kana": "コトブキチョウ",
     "alternates": []
   },
   "7478501": {
     "jis": "35206",
@@ -365940,15 +365845,15 @@
     "neighborhood": "本町",
     "banchi": "5区",
     "postal_code": "7578585",
     "old_code": "757  ",
     "post_office": "厚狭",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "",
     "city_kana": "",
     "neighborhood_kana": "",
     "alternates": []
   },
   "7578634": {
     "jis": "35216",
@@ -369439,15 +369344,15 @@
     "neighborhood": "笠木",
     "banchi": "字西野39",
     "postal_code": "7711295",
     "old_code": "77112",
     "post_office": "藍住",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "トクシマケン",
     "city_kana": "イタノグンアイズミチョウ",
     "neighborhood_kana": "カサギ",
     "alternates": []
   },
   "7711289": {
     "jis": "36403",
@@ -376401,14 +376306,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "エヒメケン",
     "city_kana": "マツヤマシ",
     "neighborhood_kana": "アンジョウジマチ",
     "alternates": []
   },
+  "7918525": {
+    "jis": "38201",
+    "kana": "カブシキガイシヤ オオサカソ-ダ マツヤマコウジヨウ",
+    "name": "株式会社　大阪ソーダ　松山工場",
+    "prefecture": "愛媛県",
+    "city": "松山市",
+    "neighborhood": "北吉田町",
+    "banchi": "77番地",
+    "postal_code": "7918525",
+    "old_code": "791  ",
+    "post_office": "松山西",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "エヒメケン",
+    "city_kana": "マツヤマシ",
+    "neighborhood_kana": "キタヨシダマチ",
+    "alternates": []
+  },
   "7918672": {
     "jis": "38201",
     "kana": "カブシキガイシヤ カナツクス",
     "name": "株式会社　カナックス",
     "prefecture": "愛媛県",
     "city": "松山市",
     "neighborhood": "姫原",
@@ -376610,33 +376534,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "エヒメケン",
     "city_kana": "マツヤマシ",
     "neighborhood_kana": "ミサワ",
     "alternates": []
   },
-  "7918525": {
-    "jis": "38201",
-    "kana": "ダイソ- カブシキガイシヤ マツヤマコウジヨウ",
-    "name": "ダイソー　株式会社　松山工場",
-    "prefecture": "愛媛県",
-    "city": "松山市",
-    "neighborhood": "北吉田町",
-    "banchi": "77",
-    "postal_code": "7918525",
-    "old_code": "791  ",
-    "post_office": "松山西",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "エヒメケン",
-    "city_kana": "マツヤマシ",
-    "neighborhood_kana": "キタヨシダマチ",
-    "alternates": []
-  },
   "7918531": {
     "jis": "38201",
     "kana": "ダイヤアルミ カブシキガイシヤ",
     "name": "ダイヤアルミ　（株）",
     "prefecture": "愛媛県",
     "city": "松山市",
     "neighborhood": "安城寺町",
@@ -378713,15 +378618,15 @@
     "neighborhood": "東大洲",
     "banchi": "1582番地",
     "postal_code": "7958506",
     "old_code": "795  ",
     "post_office": "大洲",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "エヒメケン",
     "city_kana": "オオズシ",
     "neighborhood_kana": "ヒガシオオズ",
     "alternates": []
   },
   "7958510": {
     "jis": "38207",
@@ -380486,33 +380391,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "コウチケン",
     "city_kana": "コウチシ",
     "neighborhood_kana": "ホンマチ",
     "alternates": []
   },
-  "7808662": {
-    "jis": "39201",
-    "kana": "カブシキガイシヤ コウチシンブンシヤ (パブリシテイ)",
-    "name": "株式会社　高知新聞社　（パブリシティ）",
-    "prefecture": "高知県",
-    "city": "高知市",
-    "neighborhood": "本町",
-    "banchi": "3丁目2-15",
-    "postal_code": "7808662",
-    "old_code": "780  ",
-    "post_office": "高知中央",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "コウチケン",
-    "city_kana": "コウチシ",
-    "neighborhood_kana": "ホンマチ",
-    "alternates": []
-  },
   "7808566": {
     "jis": "39201",
     "kana": "カブシキガイシヤ コウチダイマル",
     "name": "株式会社　高知大丸",
     "prefecture": "高知県",
     "city": "高知市",
     "neighborhood": "帯屋町",
@@ -383610,21 +383496,21 @@
   "8080196": {
     "jis": "40103",
     "kana": "キユウシユウコウギヨウダイガクダイガクイン セイメイタイコウガクケンキユウカ",
     "name": "九州工業大学大学院　生命体工学研究科",
     "prefecture": "福岡県",
     "city": "北九州市若松区",
     "neighborhood": "ひびきの",
-    "banchi": "1-1",
+    "banchi": "2-4",
     "postal_code": "8080196",
     "old_code": "80801",
     "post_office": "二島",
     "type": "office",
     "multiple": false,
-    "new": false,
+    "new": true,
     "prefecture_kana": "フクオカケン",
     "city_kana": "キタキュウシュウシワカマツク",
     "neighborhood_kana": "ヒビキノ",
     "alternates": []
   },
   "8048520": {
     "jis": "40105",
@@ -396938,15 +396824,15 @@
     "neighborhood": "五条",
     "banchi": "3丁目11-25(筑紫野郵便局私書箱第17号)",
     "postal_code": "8180197",
     "old_code": "81801",
     "post_office": "筑紫野",
     "type": "box",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "フクオカケン",
     "city_kana": "ダザイフシ",
     "neighborhood_kana": "ゴジョウ",
     "alternates": []
   },
   "8113197": {
     "jis": "40223",
@@ -406369,14 +406255,33 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "ハナバタチョウ",
     "alternates": []
   },
+  "8608502": {
+    "jis": "43101",
+    "kana": "ゼンコクケンコウホケンキヨウカイ クマモトシブ",
+    "name": "全国健康保険協会　熊本支部",
+    "prefecture": "熊本県",
+    "city": "熊本市中央区",
+    "neighborhood": "辛島町",
+    "banchi": "5-1日本生命熊本ビル10階",
+    "postal_code": "8608502",
+    "old_code": "860  ",
+    "post_office": "熊本中央",
+    "type": "office",
+    "multiple": false,
+    "new": true,
+    "prefecture_kana": "クマモトケン",
+    "city_kana": "クマモトシチュウオウク",
+    "neighborhood_kana": "カラシマチョウ",
+    "alternates": []
+  },
   "8608526": {
     "jis": "43101",
     "kana": "ソンガイホケンジヤパンニツポンコウア カブシキカイシヤ",
     "name": "損害保険ジャパン日本興亜　株式会社",
     "prefecture": "熊本県",
     "city": "熊本市中央区",
     "neighborhood": "花畑町",
@@ -406458,15 +406363,15 @@
     "neighborhood": "辛島町",
     "banchi": "5番1号日本生命熊本ビル9階",
     "postal_code": "8608581",
     "old_code": "860  ",
     "post_office": "熊本中央",
     "type": "office",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "カラシマチョウ",
     "alternates": []
   },
   "8608602": {
     "jis": "43101",
@@ -407129,33 +407034,14 @@
     "multiple": false,
     "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "クマモトシチュウオウク",
     "neighborhood_kana": "シンヤシキ",
     "alternates": []
   },
-  "8628520": {
-    "jis": "43101",
-    "kana": "ゼンコクケンコウホケンキヨウカイ クマモトシブ",
-    "name": "全国健康保険協会　熊本支部",
-    "prefecture": "熊本県",
-    "city": "熊本市中央区",
-    "neighborhood": "水前寺",
-    "banchi": "1丁目20-22水前寺センタービル",
-    "postal_code": "8628520",
-    "old_code": "862  ",
-    "post_office": "熊本東",
-    "type": "office",
-    "multiple": false,
-    "new": false,
-    "prefecture_kana": "クマモトケン",
-    "city_kana": "クマモトシチュウオウク",
-    "neighborhood_kana": "スイゼンジ",
-    "alternates": []
-  },
   "8628585": {
     "jis": "43101",
     "kana": "ニシニホンデンシンデンワ カブシキガイシヤ クマモトシテン",
     "name": "西日本電信電話　株式会社　熊本支店",
     "prefecture": "熊本県",
     "city": "熊本市中央区",
     "neighborhood": "九品寺",
@@ -408340,15 +408226,15 @@
     "neighborhood": "通町",
     "banchi": "10-10(八代郵便局私書箱第19号)",
     "postal_code": "8668660",
     "old_code": "866  ",
     "post_office": "八代",
     "type": "box",
     "multiple": false,
-    "new": true,
+    "new": false,
     "prefecture_kana": "クマモトケン",
     "city_kana": "ヤツシロシ",
     "neighborhood_kana": "トオリチョウ",
     "alternates": []
   },
   "8668533": {
     "jis": "43202",
```

### Comparing `posuto-2023.7.0/posuto/postaldata.db` & `posuto-2023.8.0/posuto/postaldata.db`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -6634,17 +6634,17 @@
 INSERT INTO postal_data VALUES('0800345','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800345", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "タカクラ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "高倉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','高倉');
 INSERT INTO postal_data VALUES('0800151','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800151", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "トウワ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "東和", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','東和');
 INSERT INTO postal_data VALUES('0800261','{"jisx0402": "01631", "old_code": "08002", "postal_code": "0800261", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "トカチガワオンセン", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "十勝川温泉", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','十勝川温泉');
 INSERT INTO postal_data VALUES('0800263','{"jisx0402": "01631", "old_code": "08002", "postal_code": "0800263", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "トカチガワオンセンミナミ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "十勝川温泉南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','十勝川温泉南');
 INSERT INTO postal_data VALUES('0800262','{"jisx0402": "01631", "old_code": "08002", "postal_code": "0800262", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "トカチガワオンセンキタ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "十勝川温泉北", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','十勝川温泉北');
 INSERT INTO postal_data VALUES('0800561','{"jisx0402": "01631", "old_code": "08005", "postal_code": "0800561", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "トヨタ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "豊田", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','豊田');
 INSERT INTO postal_data VALUES('0800578','{"jisx0402": "01631", "old_code": "08005", "postal_code": "0800578", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカオトフケ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中音更", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中音更');
-INSERT INTO postal_data VALUES('0800309','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800309", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカスズランモトマチ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中鈴蘭元町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中鈴蘭元町');
-INSERT INTO postal_data VALUES('0800308','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800308", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカスズランミナミ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中鈴蘭南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中鈴蘭南');
 INSERT INTO postal_data VALUES('0800307','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800307", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカスズランキタ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中鈴蘭北", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中鈴蘭北');
+INSERT INTO postal_data VALUES('0800308','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800308", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカスズランミナミ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中鈴蘭南", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中鈴蘭南');
+INSERT INTO postal_data VALUES('0800309','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800309", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナカスズランモトマチ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "中鈴蘭元町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','中鈴蘭元町');
 INSERT INTO postal_data VALUES('0800346','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800346", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ナツゾラ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "なつぞら", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','なつぞら');
 INSERT INTO postal_data VALUES('0800577','{"jisx0402": "01631", "old_code": "08005", "postal_code": "0800577", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ニシナカオトフケ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "西中音更", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','西中音更');
 INSERT INTO postal_data VALUES('0800325','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800325", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ハクジュダイ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "柏寿台", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','柏寿台');
 INSERT INTO postal_data VALUES('0800562','{"jisx0402": "01631", "old_code": "08005", "postal_code": "0800562", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ヒガシオトフケ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "東音更", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','東音更');
 INSERT INTO postal_data VALUES('0800343','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800343", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ヒガシシカリ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "東士狩", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','東士狩');
 INSERT INTO postal_data VALUES('0800106','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800106", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ヒガシドオリ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "東通", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','東通');
 INSERT INTO postal_data VALUES('0800162','{"jisx0402": "01631", "old_code": "08001", "postal_code": "0800162", "prefecture_kana": "ホッカイドウ", "city_kana": "カトウグンオトフケチョウ", "neighborhood_kana": "ヒビキノナカマチ", "prefecture": "北海道", "city": "河東郡音更町", "neighborhood": "ひびき野仲町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','北海道','河東郡音更町','ひびき野仲町');
@@ -31628,14 +31628,15 @@
 INSERT INTO postal_data VALUES('3450827','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450827", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ホンデン", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "本田", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','本田');
 INSERT INTO postal_data VALUES('3450823','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450823", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ミヤシロ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "宮代", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','宮代');
 INSERT INTO postal_data VALUES('3450835','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450835", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ミヤシロダイ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "宮代台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','宮代台');
 INSERT INTO postal_data VALUES('3450803','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450803", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ミヤヒガシ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "宮東", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','宮東');
 INSERT INTO postal_data VALUES('3450801','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450801", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "モンマ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "百間", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','百間');
 INSERT INTO postal_data VALUES('3450824','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450824", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ヤマザキ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "山崎", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','山崎');
 INSERT INTO postal_data VALUES('3450836','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450836", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ワド", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "和戸", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','和戸');
+INSERT INTO postal_data VALUES('3450837','{"jisx0402": "11442", "old_code": "345  ", "postal_code": "3450837", "prefecture_kana": "サイタマケン", "city_kana": "ミナミサイタマグンミヤシロマチ", "neighborhood_kana": "ワドヨコマチ", "prefecture": "埼玉県", "city": "南埼玉郡宮代町", "neighborhood": "和戸横町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','埼玉県','南埼玉郡宮代町','和戸横町');
 INSERT INTO postal_data VALUES('3450035','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450035", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "ウチダ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "内田", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','内田');
 INSERT INTO postal_data VALUES('3450042','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450042", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "オオジマ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "大島", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','大島');
 INSERT INTO postal_data VALUES('3450022','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450022", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "オオツカ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "大塚", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','大塚');
 INSERT INTO postal_data VALUES('3450021','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450021", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "キタハスヌマ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "北蓮沼", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','北蓮沼');
 INSERT INTO postal_data VALUES('3450001','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450001", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "キヅウチ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "木津内", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','木津内');
 INSERT INTO postal_data VALUES('3450003','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450003", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "キノカワ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "木野川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','木野川');
 INSERT INTO postal_data VALUES('3450034','{"jisx0402": "11464", "old_code": "345  ", "postal_code": "3450034", "prefecture_kana": "サイタマケン", "city_kana": "キタカツシカグンスギトマチ", "neighborhood_kana": "クラマツ", "prefecture": "埼玉県", "city": "北葛飾郡杉戸町", "neighborhood": "倉松", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','埼玉県','北葛飾郡杉戸町','倉松');
@@ -36412,14 +36413,60 @@
 INSERT INTO postal_data VALUES('1056031','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056031", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "31階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056032','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056032", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "32階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056033','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056033", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "33階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056034','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056034", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "34階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056035','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056035", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "35階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056036','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056036", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "36階"}','東京都','港区','虎ノ門城山トラストタワー');
 INSERT INTO postal_data VALUES('1056037','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056037", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモンシロヤマトラストタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門城山トラストタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "37階"}','東京都','港区','虎ノ門城山トラストタワー');
+INSERT INTO postal_data VALUES('1055590','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055590", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "地階・階層不明"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055501','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055501", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "1階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055502','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055502", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "2階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055503','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055503", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "3階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055504','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055504", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "4階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055505','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055505", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "5階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055506','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055506", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "6階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055507','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055507", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "7階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055508','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055508", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "8階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055509','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055509", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "9階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055510','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055510", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "10階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055515','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055515", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "15階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055516','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055516", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "16階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055517','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055517", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "17階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055518','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055518", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "18階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055519','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055519", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "19階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055520','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055520", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "20階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055521','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055521", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "21階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055522','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055522", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "22階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055523','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055523", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "23階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055524','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055524", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "24階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055525','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055525", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "25階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055526','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055526", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "26階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055527','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055527", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "27階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055528','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055528", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "28階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055529','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055529", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "29階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055530','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055530", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "30階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055531','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055531", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "31階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055532','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055532", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "32階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055533','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055533", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "33階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055534','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055534", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "34階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055535','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055535", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "35階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055536','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055536", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "36階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055537','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055537", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "37階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055538','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055538", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "38階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055539','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055539", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "39階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055540','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055540", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "40階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055541','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055541", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "41階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055542','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055542", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "42階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055543','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055543", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "43階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055544','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055544", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "44階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055545','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055545", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "45階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055546','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055546", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "46階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055547','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055547", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "47階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055548','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055548", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "48階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
+INSERT INTO postal_data VALUES('1055549','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1055549", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズステーションタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズステーションタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": "49階"}','東京都','港区','虎ノ門虎ノ門ヒルズステーションタワー');
 INSERT INTO postal_data VALUES('1056490','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056490", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "地階・階層不明"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056401','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056401", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "1階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056402','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056402", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "2階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056403','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056403", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "3階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056404','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056404", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "4階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056405','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056405", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "5階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
 INSERT INTO postal_data VALUES('1056406','{"jisx0402": "13103", "old_code": "105  ", "postal_code": "1056406", "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "トラノモントラノモンヒルズビジネスタワー", "prefecture": "東京都", "city": "港区", "neighborhood": "虎ノ門虎ノ門ヒルズビジネスタワー", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "6階"}','東京都','港区','虎ノ門虎ノ門ヒルズビジネスタワー');
@@ -66248,14 +66295,15 @@
 INSERT INTO postal_data VALUES('4890879','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890879", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "コブキチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "瘤木町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','瘤木町');
 INSERT INTO postal_data VALUES('4890974','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890974", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "コママエチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "駒前町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','駒前町');
 INSERT INTO postal_data VALUES('4890035','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890035", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "コンヤダチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "紺屋田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','紺屋田町');
 INSERT INTO postal_data VALUES('4890818','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890818", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "サイワイチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "幸町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','幸町');
 INSERT INTO postal_data VALUES('4890977','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890977", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "サカウエチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "坂上町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','坂上町');
 INSERT INTO postal_data VALUES('4890044','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890044", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "サカエマチ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "栄町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','栄町');
 INSERT INTO postal_data VALUES('4890982','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890982", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "サツキダイ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "さつき台", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','さつき台');
+INSERT INTO postal_data VALUES('4890899','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890899", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シオクサガオカ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "塩草が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "区画整理", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','塩草が丘');
 INSERT INTO postal_data VALUES('4890895','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890895", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シオクサチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "塩草町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','塩草町');
 INSERT INTO postal_data VALUES('4890901','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890901", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "ジッケンチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "十軒町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','十軒町');
 INSERT INTO postal_data VALUES('4801207','{"jisx0402": "23204", "old_code": "48012", "postal_code": "4801207", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シナノチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "品野町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','品野町');
 INSERT INTO postal_data VALUES('4890051','{"jisx0402": "23204", "old_code": "489  ", "postal_code": "4890051", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シモジンヤチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "下陣屋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','下陣屋町');
 INSERT INTO postal_data VALUES('4801202','{"jisx0402": "23204", "old_code": "48012", "postal_code": "4801202", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シモハダガワチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "下半田川町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','下半田川町');
 INSERT INTO postal_data VALUES('4801201','{"jisx0402": "23204", "old_code": "48012", "postal_code": "4801201", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "ジョウコウジチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "定光寺町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','定光寺町');
 INSERT INTO postal_data VALUES('4801213','{"jisx0402": "23204", "old_code": "48012", "postal_code": "4801213", "prefecture_kana": "アイチケン", "city_kana": "セトシ", "neighborhood_kana": "シライワチョウ", "prefecture": "愛知県", "city": "瀬戸市", "neighborhood": "白岩町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','愛知県','瀬戸市','白岩町');
@@ -74214,25 +74262,25 @@
 INSERT INTO postal_data VALUES('5280006','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280006", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウモトマチ", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町元町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町元町');
 INSERT INTO postal_data VALUES('5280032','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280032", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウヤサカ", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町八坂", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町八坂');
 INSERT INTO postal_data VALUES('5280067','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280067", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウヤマ", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町山');
 INSERT INTO postal_data VALUES('5280044','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280044", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウヤマガミ", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町山上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町山上');
 INSERT INTO postal_data VALUES('5280014','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280014", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウロクシン", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町鹿深", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町鹿深');
 INSERT INTO postal_data VALUES('5280003','{"jisx0402": "25209", "old_code": "528  ", "postal_code": "5280003", "prefecture_kana": "シガケン", "city_kana": "コウカシ", "neighborhood_kana": "ミナクチチョウワノ", "prefecture": "滋賀県", "city": "甲賀市", "neighborhood": "水口町和野", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','甲賀市','水口町和野');
 INSERT INTO postal_data VALUES('5202300','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202300", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','滋賀県','野洲市','');
-INSERT INTO postal_data VALUES('5240202','{"jisx0402": "25210", "old_code": "52402", "postal_code": "5240202", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "アヤメ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "菖蒲", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','菖蒲');
+INSERT INTO postal_data VALUES('5202402','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202402", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "アヤメ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "菖蒲", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "郵便区調整等", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','菖蒲');
 INSERT INTO postal_data VALUES('5202411','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202411", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "アワジ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "安治", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','安治');
 INSERT INTO postal_data VALUES('5202362','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202362", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "イチミヤケ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "市三宅", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','市三宅');
 INSERT INTO postal_data VALUES('5202414','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202414", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "イノクチ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "井口", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','井口');
 INSERT INTO postal_data VALUES('5202312','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202312", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "イリマチ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "入町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','入町');
 INSERT INTO postal_data VALUES('5202324','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202324", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "オウミフジ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "近江富士", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','近江富士');
 INSERT INTO postal_data VALUES('5202313','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202313", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "オオシノハラ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "大篠原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','大篠原');
 INSERT INTO postal_data VALUES('5202343','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202343", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "オオハタ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "大畑", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','大畑');
 INSERT INTO postal_data VALUES('5202435','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202435", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "オチクボ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "乙窪", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','乙窪');
 INSERT INTO postal_data VALUES('5202316','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202316", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "カミヤ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "上屋", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','上屋');
-INSERT INTO postal_data VALUES('5240203','{"jisx0402": "25210", "old_code": "52402", "postal_code": "5240203", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キゴウ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "喜合", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','喜合');
+INSERT INTO postal_data VALUES('5202403','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202403", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キゴウ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "喜合", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "郵便区調整等", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','喜合');
 INSERT INTO postal_data VALUES('5202305','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202305", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キタ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "北", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','北');
 INSERT INTO postal_data VALUES('5202321','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202321", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キタザクラ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "北桜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','北桜');
 INSERT INTO postal_data VALUES('5202361','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202361", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キタノ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "北野", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','北野');
 INSERT INTO postal_data VALUES('5202436','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202436", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キタヒエ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "北比江", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','北比江');
 INSERT INTO postal_data VALUES('5202431','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202431", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "キベ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "木部", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','木部');
 INSERT INTO postal_data VALUES('5202353','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202353", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "クノベ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "久野部", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','久野部');
 INSERT INTO postal_data VALUES('5202331','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202331", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "コシノハラ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "小篠原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','小篠原');
@@ -74261,15 +74309,15 @@
 INSERT INTO postal_data VALUES('5202323','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202323", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ミカミ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "三上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','三上');
 INSERT INTO postal_data VALUES('5202322','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202322", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ミナミザクラ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "南桜", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','南桜');
 INSERT INTO postal_data VALUES('5202332','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202332", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ミョウコウジ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "妙光寺", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','妙光寺');
 INSERT INTO postal_data VALUES('5202432','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202432", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ムシュウ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "虫生", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','虫生');
 INSERT INTO postal_data VALUES('5202342','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202342", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヤス", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "野洲", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','野洲');
 INSERT INTO postal_data VALUES('5202433','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202433", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヤブ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "八夫", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','八夫');
 INSERT INTO postal_data VALUES('5202341','{"jisx0402": "25210", "old_code": "52023", "postal_code": "5202341", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ユキハタ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "行畑", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','行畑');
-INSERT INTO postal_data VALUES('5240201','{"jisx0402": "25210", "old_code": "52402", "postal_code": "5240201", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヨシカワ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "吉川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','吉川');
+INSERT INTO postal_data VALUES('5202401','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202401", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヨシカワ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "吉川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "郵便区調整等", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','吉川');
 INSERT INTO postal_data VALUES('5202413','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202413", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ヨシジ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "吉地", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','吉地');
 INSERT INTO postal_data VALUES('5202412','{"jisx0402": "25210", "old_code": "52024", "postal_code": "5202412", "prefecture_kana": "シガケン", "city_kana": "ヤスシ", "neighborhood_kana": "ロクジョウ", "prefecture": "滋賀県", "city": "野洲市", "neighborhood": "六条", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','野洲市','六条');
 INSERT INTO postal_data VALUES('5203200','{"jisx0402": "25211", "old_code": "52032", "postal_code": "5203200", "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','滋賀県','湖南市','');
 INSERT INTO postal_data VALUES('5203251','{"jisx0402": "25211", "old_code": "52032", "postal_code": "5203251", "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "アサクニ", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "朝国", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','湖南市','朝国');
 INSERT INTO postal_data VALUES('5203116','{"jisx0402": "25211", "old_code": "52031", "postal_code": "5203116", "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "アメヤマ", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "雨山", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','湖南市','雨山');
 INSERT INTO postal_data VALUES('5203101','{"jisx0402": "25211", "old_code": "52031", "postal_code": "5203101", "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベ", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','湖南市','石部');
 INSERT INTO postal_data VALUES('5203109','{"jisx0402": "25211", "old_code": "52031", "postal_code": "5203109", "prefecture_kana": "シガケン", "city_kana": "コナンシ", "neighborhood_kana": "イシベガオカ", "prefecture": "滋賀県", "city": "湖南市", "neighborhood": "石部が丘", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','滋賀県','湖南市','石部が丘');
@@ -110364,14 +110412,15 @@
 INSERT INTO postal_data VALUES('8112309','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112309", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "カヨイチョウ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "駕与丁", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','駕与丁');
 INSERT INTO postal_data VALUES('8112315','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112315", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "コウナカバル", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "甲仲原", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','甲仲原');
 INSERT INTO postal_data VALUES('8112303','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112303", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "サカド", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "酒殿", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','酒殿');
 INSERT INTO postal_data VALUES('8112311','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112311", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "チョウジャバル", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "長者原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','長者原');
 INSERT INTO postal_data VALUES('8112316','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112316", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "チョウジャバルニシ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "長者原西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','長者原西');
 INSERT INTO postal_data VALUES('8112317','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112317", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "チョウジャバルヒガシ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "長者原東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','長者原東');
 INSERT INTO postal_data VALUES('8112312','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112312", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "トバラ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "戸原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','戸原');
+INSERT INTO postal_data VALUES('8112322','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112322", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "トバラキタ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "戸原北", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更あり", "update_reason": "住居表示の実施", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','戸原北');
 INSERT INTO postal_data VALUES('8112319','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112319", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "トバラニシ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "戸原西", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','戸原西');
 INSERT INTO postal_data VALUES('8112318','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112318", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "トバラヒガシ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "戸原東", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','戸原東');
 INSERT INTO postal_data VALUES('8112304','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112304", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "ナカバル", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "仲原", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','仲原');
 INSERT INTO postal_data VALUES('8112310','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112310", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "ハナガウラ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "花ヶ浦", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','花ヶ浦');
 INSERT INTO postal_data VALUES('8112307','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112307", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "ハルマチ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "原町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','原町');
 INSERT INTO postal_data VALUES('8112305','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112305", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "ユス", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "柚須", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','柚須');
 INSERT INTO postal_data VALUES('8112314','{"jisx0402": "40349", "old_code": "81123", "postal_code": "8112314", "prefecture_kana": "フクオカケン", "city_kana": "カスヤグンカスヤマチ", "neighborhood_kana": "ワカミヤ", "prefecture": "福岡県", "city": "糟屋郡粕屋町", "neighborhood": "若宮", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','福岡県','糟屋郡粕屋町','若宮');
@@ -118930,35 +118979,35 @@
 INSERT INTO postal_data VALUES('8996301','{"jisx0402": "46218", "old_code": "89963", "postal_code": "8996301", "prefecture_kana": "カゴシマケン", "city_kana": "キリシマシ", "neighborhood_kana": "ヨコガワチョウカミノ", "prefecture": "鹿児島県", "city": "霧島市", "neighborhood": "横川町上ノ", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','霧島市','横川町上ノ');
 INSERT INTO postal_data VALUES('8996302','{"jisx0402": "46218", "old_code": "89963", "postal_code": "8996302", "prefecture_kana": "カゴシマケン", "city_kana": "キリシマシ", "neighborhood_kana": "ヨコガワチョウシモノ", "prefecture": "鹿児島県", "city": "霧島市", "neighborhood": "横川町下ノ", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','霧島市','横川町下ノ');
 INSERT INTO postal_data VALUES('8996303','{"jisx0402": "46218", "old_code": "89963", "postal_code": "8996303", "prefecture_kana": "カゴシマケン", "city_kana": "キリシマシ", "neighborhood_kana": "ヨコガワチョウナカノ", "prefecture": "鹿児島県", "city": "霧島市", "neighborhood": "横川町中ノ", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','霧島市','横川町中ノ');
 INSERT INTO postal_data VALUES('8960000','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960000", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": "以下に掲載がない場合"}','鹿児島県','いちき串木野市','');
 INSERT INTO postal_data VALUES('8960061','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960061", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アイギチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "愛木町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','愛木町');
 INSERT INTO postal_data VALUES('8960001','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960001", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アケボノチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "曙町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','曙町');
 INSERT INTO postal_data VALUES('8960015','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960015", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アサヒマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "旭町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','旭町');
-INSERT INTO postal_data VALUES('8960084','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960084", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アサヤマ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "浅山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','浅山');
+INSERT INTO postal_data VALUES('8960084','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960084", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アサヤマ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "浅山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','浅山');
 INSERT INTO postal_data VALUES('8960065','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960065", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "アラカワ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "荒川", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','荒川');
 INSERT INTO postal_data VALUES('8960036','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960036", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ウラワチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "浦和町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','浦和町');
 INSERT INTO postal_data VALUES('8960027','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960027", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "エビスチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "恵比須町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','恵比須町');
 INSERT INTO postal_data VALUES('8992103','{"jisx0402": "46219", "old_code": "89921", "postal_code": "8992103", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "オオザト", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "大里", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','大里');
-INSERT INTO postal_data VALUES('8960081','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960081", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "オオゾノ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "大薗", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','大薗');
+INSERT INTO postal_data VALUES('8960081','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960081", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "オオゾノ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "大薗", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','大薗');
 INSERT INTO postal_data VALUES('8960011','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960011", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "オオハルマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "大原町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','大原町');
 INSERT INTO postal_data VALUES('8960025','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960025", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "オクラチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "御倉町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','御倉町');
 INSERT INTO postal_data VALUES('8960057','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960057", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カイゼ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "海瀬", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','海瀬');
 INSERT INTO postal_data VALUES('8960002','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960002", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カスガチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "春日町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','春日町');
 INSERT INTO postal_data VALUES('8960079','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960079", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カワウチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "河内", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','河内');
 INSERT INTO postal_data VALUES('8992102','{"jisx0402": "46219", "old_code": "89921", "postal_code": "8992102", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カワカミ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "川上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','川上');
 INSERT INTO postal_data VALUES('8960052','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960052", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カンミョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "上名", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','上名');
 INSERT INTO postal_data VALUES('8960051','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960051", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "カンムリダケ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "冠嶽", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','冠嶽');
 INSERT INTO postal_data VALUES('8960041','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960041", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "キタハマチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "北浜町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','北浜町');
 INSERT INTO postal_data VALUES('8960003','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960003", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "キョウマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "京町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','京町');
 INSERT INTO postal_data VALUES('8960075','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960075", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "キンザン", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "金山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','金山');
 INSERT INTO postal_data VALUES('8960074','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960074", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "キンザンシモ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "金山下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','金山下');
 INSERT INTO postal_data VALUES('8960063','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960063", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "クチノマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "口之町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','口之町');
 INSERT INTO postal_data VALUES('8960034','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960034", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "コゼチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "小瀬町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','小瀬町');
-INSERT INTO postal_data VALUES('8960082','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960082", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "コゾノ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "小薗", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','小薗');
+INSERT INTO postal_data VALUES('8960082','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960082", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "コゾノ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "小薗", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','小薗');
 INSERT INTO postal_data VALUES('8960013','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960013", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "サカエマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "栄町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','栄町');
 INSERT INTO postal_data VALUES('8960016','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960016", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "サクラマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "桜町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','桜町');
 INSERT INTO postal_data VALUES('8960072','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960072", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "サツマヤマ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "薩摩山", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','薩摩山');
 INSERT INTO postal_data VALUES('8960004','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960004", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "シオミチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "汐見町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','汐見町');
 INSERT INTO postal_data VALUES('8960023','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960023", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "シオヤチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "塩屋町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','塩屋町');
 INSERT INTO postal_data VALUES('8960026','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960026", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ショウワドオリ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "昭和通", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','昭和通');
 INSERT INTO postal_data VALUES('8960035','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960035", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "シンセイチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "新生町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','新生町');
@@ -118982,15 +119031,15 @@
 INSERT INTO postal_data VALUES('8960006','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960006", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ヒガシエンデンチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "東塩田町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','東塩田町');
 INSERT INTO postal_data VALUES('8960031','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960031", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ヒガシシマビラチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "東島平町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','東島平町');
 INSERT INTO postal_data VALUES('8960054','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960054", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ヒノデチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "日出町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','日出町');
 INSERT INTO postal_data VALUES('8960028','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960028", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ヒバリガオカ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "ひばりが丘", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','ひばりが丘');
 INSERT INTO postal_data VALUES('8960067','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960067", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ヒラエ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "平江", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','平江');
 INSERT INTO postal_data VALUES('8960071','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960071", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "フカタカミ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "深田上", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','深田上');
 INSERT INTO postal_data VALUES('8960077','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960077", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "フカタシモ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "深田下", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','深田下');
-INSERT INTO postal_data VALUES('8960083','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960083", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "フモト", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "麓", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更あり", "update_reason": "訂正", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','麓');
+INSERT INTO postal_data VALUES('8960083','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960083", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "フモト", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "麓", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','麓');
 INSERT INTO postal_data VALUES('8960037','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960037", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ベップ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "別府", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','別府');
 INSERT INTO postal_data VALUES('8960045','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960045", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "マグロホンマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "まぐろ本町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','まぐろ本町');
 INSERT INTO postal_data VALUES('8960024','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960024", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ミスミチョウ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "美住町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','美住町');
 INSERT INTO postal_data VALUES('8960068','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960068", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ミツイ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "三井", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','三井');
 INSERT INTO postal_data VALUES('8960022','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960022", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ミドリマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "緑町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','緑町');
 INSERT INTO postal_data VALUES('8960043','{"jisx0402": "46219", "old_code": "896  ", "postal_code": "8960043", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ミナトマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "港町", "partial": false, "koazabanchi": false, "chome": false, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','港町');
 INSERT INTO postal_data VALUES('8992101','{"jisx0402": "46219", "old_code": "89921", "postal_code": "8992101", "prefecture_kana": "カゴシマケン", "city_kana": "イチキクシキノシ", "neighborhood_kana": "ミナトマチ", "prefecture": "鹿児島県", "city": "いちき串木野市", "neighborhood": "湊町", "partial": false, "koazabanchi": false, "chome": true, "multi": false, "update_status": "変更なし", "update_reason": "変更なし", "multiline": false, "alternates": [], "note": null}','鹿児島県','いちき串木野市','湊町');
@@ -120464,15 +120513,15 @@
 INSERT INTO office_data VALUES('0608667','{"jis": "01101", "kana": "カブシキガイシヤ サツポロマルイミツコシ マルイイマイサツポロホンテン", "name": "株式会社　札幌丸井三越　丸井今井札幌本店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "2丁目11", "postal_code": "0608667", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608623','{"jis": "01101", "kana": "カブシキガイシヤ ジエ-シ-ビ- ホツカイドウシシヤ", "name": "株式会社　ジェーシービー　北海道支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "1丁目1番地JCB札幌東ビル", "postal_code": "0608623", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608577','{"jis": "01101", "kana": "カブシキガイシヤ ジヤツクス サツポロシシヤ", "name": "株式会社　ジャックス　札幌支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "6丁目1-2アーバンネット札幌ビル5F", "postal_code": "0608577", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608533','{"jis": "01101", "kana": "カブシキガイシヤ スズケン", "name": "株式会社　スズケン", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北十一条西", "banchi": "19丁目36番35号", "postal_code": "0608533", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608512','{"jis": "01101", "kana": "カブシキガイシヤ ソワン・エフ", "name": "（株）　ソワン・エフ", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "12丁目4番地扶洋第一ビル", "postal_code": "0608512", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": [{"jis": "01101", "kana": "カブシキガイシヤ フヨウサキナ", "name": "株式会社　フヨウサキナ", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "12丁目4番地扶洋第一ビル", "postal_code": "0608512", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}, {"jis": "01101", "kana": "フヨウエステ-ト カブシキガイシヤ", "name": "扶洋エステート　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "12丁目4番地扶洋第一ビル", "postal_code": "0608512", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}, {"jis": "01101", "kana": "フヨウマネ-ジメントサ-ビス カブシキガイシヤ", "name": "扶洋マネージメントサービス　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "12丁目4番地扶洋第一ビル", "postal_code": "0608512", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}, {"jis": "01101", "kana": "フヨウヤクヒン カブシキガイシヤ", "name": "扶洋薬品　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "12丁目4番地扶洋第一ビル", "postal_code": "0608512", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}]}');
 INSERT INTO office_data VALUES('0608536','{"jis": "01101", "kana": "カブシキガイシヤ テイコクデ-タバンク サツポロシテン", "name": "（株）　帝国データバンク　札幌支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南二条西", "banchi": "9丁目1-17", "postal_code": "0608536", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608545','{"jis": "01101", "kana": "カブシキガイシヤ デンツウホツカイドウ", "name": "株式会社　電通北海道", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "5丁目11-1", "postal_code": "0608545", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
-INSERT INTO office_data VALUES('0608529','{"jis": "01101", "kana": "カブシキガイシヤ ニツプン サツポロシテン", "name": "株式会社　ニップン　札幌支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "5丁目2番地北1条三井ビルディング5F", "postal_code": "0608529", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
+INSERT INTO office_data VALUES('0608529','{"jis": "01101", "kana": "カブシキガイシヤ ニツプン サツポロシテン", "name": "株式会社　ニップン　札幌支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "5丁目2番地北1条三井ビルディング5F", "postal_code": "0608529", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608580','{"jis": "01101", "kana": "カブシキガイシヤ ニトリパブリツク", "name": "株式会社　ニトリパブリック", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条東", "banchi": "1丁目2", "postal_code": "0608580", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608502','{"jis": "01101", "kana": "カブシキガイシヤ パルコ サツポロテン", "name": "株式会社　パルコ　札幌店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "3丁目", "postal_code": "0608502", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608688','{"jis": "01101", "kana": "カブシキガイシヤ ベネツセコ-ポレ-シヨン ホツカイドウジギヨウシヨ", "name": "（株）　ベネッセコーポレーション　北海道事業所", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北五条西", "banchi": "2丁目JRタワーオフィスプラザさっぽろ13階", "postal_code": "0608688", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": true, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ５ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608687','{"jis": "01101", "kana": "カブシキガイシヤ ベネツセコ-ポレ-シヨン ホツカイドウジギヨウシヨ", "name": "（株）　ベネッセコーポレーション　北海道事業所", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北五条西", "banchi": "2丁目JRタワーオフィスプラザさっぽろ13階", "postal_code": "0608687", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": true, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ５ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608686','{"jis": "01101", "kana": "カブシキガイシヤ ベネツセコ-ポレ-シヨン ホツカイドウジギヨウシヨ", "name": "（株）　ベネッセコーポレーション　北海道事業所", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北五条西", "banchi": "2丁目JRタワーオフィスプラザさっぽろ13階", "postal_code": "0608686", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": true, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ５ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608565','{"jis": "01101", "kana": "カブシキガイシヤ ホクセン", "name": "株式会社　ほくせん", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南二条西", "banchi": "1丁目3北専ビル", "postal_code": "0608565", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608661','{"jis": "01101", "kana": "カブシキガイシヤ ホクヨウギンコウ ホンテン", "name": "株式会社　北洋銀行　本店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "3丁目7番地(札幌中央郵便局私書箱第121号)", "postal_code": "0608661", "old_code": "060  ", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
@@ -120521,15 +120570,15 @@
 INSERT INTO office_data VALUES('0608531','{"jis": "01101", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "3丁目7番地北洋大通センター15F~17F", "postal_code": "0608531", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608535','{"jis": "01101", "kana": "トダケンセツ カブシキガイシヤ サツポロシテン", "name": "戸田建設　株式会社　札幌支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条東", "banchi": "2丁目2", "postal_code": "0608535", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608608','{"jis": "01101", "kana": "ドウギンカ-ド カブシキカイシヤ", "name": "道銀カード　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南二条西", "banchi": "2丁目14番地", "postal_code": "0608608", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ２ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608776','{"jis": "01101", "kana": "ドウシンブンブンクラブ<フレ-ツ!フレ-ツ!キヤンペ-ン>ジムキヨク", "name": "道新ぶんぶんクラブ「フレーっ！フレーっ！キャンペーン」事務局", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "3丁目6", "postal_code": "0608776", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608618','{"jis": "01101", "kana": "ナカミチキカイ カブシキガイシヤ", "name": "中道機械　（株）", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条東", "banchi": "3丁目3番地", "postal_code": "0608618", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608539','{"jis": "01101", "kana": "ナカミチリ-ス カブシキガイシヤ", "name": "中道リース　株式会社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条東", "banchi": "3丁目3番地", "postal_code": "0608539", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608585','{"jis": "01101", "kana": "ニツポンネンキンキコウ サツポロニシネンキンジムシヨ", "name": "日本年金機構　札幌西年金事務所", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "11丁目2番1号", "postal_code": "0608585", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
-INSERT INTO office_data VALUES('0608678','{"jis": "01101", "kana": "ニホンセイメイホケン ソウゴガイシヤ サツポロシシヤ", "name": "日本生命保険　相互会社　札幌支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北四条西", "banchi": "5丁目1番3号(札幌中央郵便局私書箱第126号)", "postal_code": "0608678", "old_code": "060  ", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ４ジョウニシ", "alternates": []}');
+INSERT INTO office_data VALUES('0608678','{"jis": "01101", "kana": "ニホンセイメイホケン ソウゴガイシヤ サツポロシシヤ", "name": "日本生命保険　相互会社　札幌支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "4丁目1-1(札幌中央郵便局私書箱第126号)", "postal_code": "0608678", "old_code": "060  ", "post_office": "札幌中央", "type": "box", "multiple": false, "new": true, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608616','{"jis": "01101", "kana": "ニホンロウドウクミアイ ソウレンゴウカイ ホツカイドウレンゴウカイ", "name": "日本労働組合　総連合会　北海道連合会", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北四条西", "banchi": "12丁目ほくろうビル6階", "postal_code": "0608616", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ４ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608519','{"jis": "01101", "kana": "ヒガシニホンデンシンデンワ カブシキカイシヤ ホツカイドウシテン", "name": "東日本電信電話　株式会社　北海道支店", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北一条西", "banchi": "4丁目2番地4NTT大通4丁目ビル", "postal_code": "0608519", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608624','{"jis": "01101", "kana": "ヒタチキヤピタル カブシキガイシヤ ホツカイドウエイギヨウホンブ", "name": "日立キャピタル　（株）　北海道営業本部", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "大通西", "banchi": "3丁目11番地", "postal_code": "0608624", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "オオドオリニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608635','{"jis": "01101", "kana": "フジカサイカイジヨウホケン カブシキガイシヤ ホツカイドウホンブ", "name": "富士火災海上保険　（株）　北海道本部", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "南一条西", "banchi": "6丁目20番1号", "postal_code": "0608635", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "ミナミ１ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608504','{"jis": "01101", "kana": "フジツウ カブシキガイシヤ ホツカイドウシシヤ", "name": "富士通　株式会社　北海道支社", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北２条西", "banchi": "4丁目1番地札幌三井JPビルディング", "postal_code": "0608504", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0608558','{"jis": "01101", "kana": "ホツカイドウ イシカリシチヨウ", "name": "北海道　石狩支庁", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北三条西", "banchi": "7丁目", "postal_code": "0608558", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ３ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608541','{"jis": "01101", "kana": "ホツカイドウカイハツキヨク イシカリガワカイハツケンセツブ", "name": "北海道開発局　石狩川開発建設部", "prefecture": "北海道", "city": "札幌市中央区", "neighborhood": "北二条西", "banchi": "19丁目", "postal_code": "0608541", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシチュウオウク", "neighborhood_kana": "キタ２ジョウニシ", "alternates": []}');
@@ -120666,14 +120715,15 @@
 INSERT INTO office_data VALUES('0608566','{"jis": "01102", "kana": "ホツカイドウロウドウキヨク", "name": "北海道労働局", "prefecture": "北海道", "city": "札幌市北区", "neighborhood": "北八条西", "banchi": "2丁目第一合同庁舎", "postal_code": "0608566", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシキタク", "neighborhood_kana": "キタ８ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608655','{"jis": "01102", "kana": "ドウエイシギヨウ カブシキガイシヤ (コアレツクス)", "name": "道栄紙業　株式会社　（コアレックス）", "prefecture": "北海道", "city": "札幌市北区", "neighborhood": "北七条西", "banchi": "9丁目2-11(札幌中央郵便局私書箱第224号)", "postal_code": "0608655", "old_code": "06091", "post_office": "札幌中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシキタク", "neighborhood_kana": "キタ７ジョウニシ", "alternates": []}');
 INSERT INTO office_data VALUES('0078503','{"jis": "01103", "kana": "オカダマチユウトンチ", "name": "丘珠駐屯地", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "丘珠町", "banchi": "161番地", "postal_code": "0078503", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "オカダマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078501','{"jis": "01103", "kana": "オリヒロ (カブ) サツポロエイギヨウシヨ", "name": "オリヒロ　（株）　札幌営業所", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "北三十六条東", "banchi": "23丁目6番6号", "postal_code": "0078501", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "キタ３６ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0078733','{"jis": "01103", "kana": "キタガスジエネツクス カブシキガイシヤ", "name": "北ガスジェネックス　株式会社", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "伏古八条", "banchi": "2丁目7-1", "postal_code": "0078733", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "フシコ８ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078505','{"jis": "01103", "kana": "キンイキヨウ チユウオウビヨウイン", "name": "勤医協　中央病院", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂５条", "banchi": "1丁目9-1", "postal_code": "0078505", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0078632','{"jis": "01103", "kana": "サツポロニツサンジドウシヤ カブシキガイシヤ ヒガシナエボテン", "name": "札幌日産自動車　株式会社　東苗穂店", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂二条", "banchi": "3丁目2-5", "postal_code": "0078632", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "ヒガシナエボ２ジョウ", "alternates": []}');
+INSERT INTO office_data VALUES('0078511','{"jis": "01103", "kana": "サツラクノウギヨウキヨウドウクミアイ シニユウジギヨウブ", "name": "サツラク農業協同組合　市乳事業部", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "丘珠町", "banchi": "573-27", "postal_code": "0078511", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "オカダマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078508','{"jis": "01103", "kana": "センシユウデンギヨウ カブシキカイシヤ サツポロシテン", "name": "泉州電業　株式会社　札幌支店", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂三条", "banchi": "2丁目2番7号", "postal_code": "0078508", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "ヒガシナエボ３ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078553','{"jis": "01103", "kana": "トラスコナカヤマ カブシキガイシヤ", "name": "トラスコ中山　株式会社", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂五条", "banchi": "3丁目4番51号", "postal_code": "0078553", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "ヒガシナエボ５ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078585','{"jis": "01103", "kana": "ホツカイドウサツポロトウリヨウコウトウガツコウ", "name": "北海道札幌東陵高等学校", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂十条", "banchi": "1丁目2番21号", "postal_code": "0078585", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "ヒガシナエボ１０ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0078507','{"jis": "01103", "kana": "ホツカイドウヒノジドウシヤ カブシキガイシヤ", "name": "北海道日野自動車　（株）", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "東苗穂二条", "banchi": "3丁目2番15号", "postal_code": "0078507", "old_code": "007  ", "post_office": "丘珠", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "ヒガシナエボ２ジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('0608576','{"jis": "01103", "kana": "カブシキガイシヤ キムラ", "name": "株式会社　キムラ", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "北六条東", "banchi": "4丁目1番地7", "postal_code": "0608576", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "キタ６ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608569','{"jis": "01103", "kana": "カブシキガイシヤ タンバヤ", "name": "株式会社　丹波屋", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "北六条東", "banchi": "4丁目1番地7デ・アウネさっぽろ8F・9F", "postal_code": "0608569", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "キタ６ジョウヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('0608582','{"jis": "01103", "kana": "カブシキガイシヤ リンユウカンコウ", "name": "（株）　りんゆう観光", "prefecture": "北海道", "city": "札幌市東区", "neighborhood": "北九条東", "banchi": "2丁目40番地23", "postal_code": "0608582", "old_code": "060  ", "post_office": "札幌中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "サッポロシヒガシク", "neighborhood_kana": "キタ９ジョウヒガシ", "alternates": []}');
@@ -121223,15 +121273,15 @@
 INSERT INTO office_data VALUES('0591393','{"jis": "01213", "kana": "トヨタジドウシヤホツカイドウ カブシキガイシヤ", "name": "トヨタ自動車北海道　株式会社", "prefecture": "北海道", "city": "苫小牧市", "neighborhood": "字勇払", "banchi": "145-1", "postal_code": "0591393", "old_code": "05913", "post_office": "苫小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0591396','{"jis": "01213", "kana": "トヨタツウシヨウ カブシキガイシヤ ホツカイドウシテン", "name": "豊田通商　株式会社　北海道支店", "prefecture": "北海道", "city": "苫小牧市", "neighborhood": "字勇払", "banchi": "145-259", "postal_code": "0591396", "old_code": "05913", "post_office": "苫小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0591395','{"jis": "01213", "kana": "ニホンセイシ カブシキガイシヤ ユウフツコウジヨウ", "name": "日本製紙　（株）　勇払工場", "prefecture": "北海道", "city": "苫小牧市", "neighborhood": "字勇払", "banchi": "143番地", "postal_code": "0591395", "old_code": "05913", "post_office": "苫小牧", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('0978555','{"jis": "01214", "kana": "シリツワツカナイビヨウイン", "name": "市立稚内病院", "prefecture": "北海道", "city": "稚内市", "neighborhood": "中央", "banchi": "4丁目11-6", "postal_code": "0978555", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('0978558','{"jis": "01214", "kana": "ホツカイドウ ソウヤソウゴウシンコウキヨク", "name": "北海道　宗谷総合振興局", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目2-27", "postal_code": "0978558", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0978525','{"jis": "01214", "kana": "ホツカイドウ ワツカナイホケンジヨ", "name": "北海道　稚内保健所", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目2番27号", "postal_code": "0978525", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0978639','{"jis": "01214", "kana": "ホツカイドウキヨウイクチヨウ ソウヤキヨウイクキヨク", "name": "北海道教育庁　宗谷教育局", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目2-27", "postal_code": "0978639", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
-INSERT INTO office_data VALUES('0978678','{"jis": "01214", "kana": "ホツカイドウワツカナイコウトウガツコウ", "name": "北海道稚内高等学校", "prefecture": "北海道", "city": "稚内市", "neighborhood": "栄", "banchi": "1丁目4番1号", "postal_code": "0978678", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "サカエ", "alternates": []}');
+INSERT INTO office_data VALUES('0978678','{"jis": "01214", "kana": "ホツカイドウワツカナイコウトウガツコウ", "name": "北海道稚内高等学校", "prefecture": "北海道", "city": "稚内市", "neighborhood": "栄", "banchi": "1丁目4番1号", "postal_code": "0978678", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "サカエ", "alternates": []}');
 INSERT INTO office_data VALUES('0978527','{"jis": "01214", "kana": "ワツカナイカイハツケンセツブ", "name": "稚内開発建設部", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "5丁目6-1稚内地方合同庁舎内", "postal_code": "0978527", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0978609','{"jis": "01214", "kana": "ワツカナイコウキヨウシヨクギヨウアンテイシヨ", "name": "稚内公共職業安定所", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目1番25号", "postal_code": "0978609", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0978686','{"jis": "01214", "kana": "ワツカナイシヤクシヨ", "name": "稚内市役所", "prefecture": "北海道", "city": "稚内市", "neighborhood": "中央", "banchi": "3丁目13-15(稚内郵便局私書箱第60号)", "postal_code": "0978686", "old_code": "097  ", "post_office": "稚内", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('0978666','{"jis": "01214", "kana": "ワツカナイシンヨウキンコ ホンテン", "name": "稚内信用金庫　本店", "prefecture": "北海道", "city": "稚内市", "neighborhood": "中央", "banchi": "3丁目9-6(稚内郵便局私書箱第5号)", "postal_code": "0978666", "old_code": "097  ", "post_office": "稚内", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('0978585','{"jis": "01214", "kana": "ワツカナイドボクゲンギヨウシヨ", "name": "稚内土木現業所", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目2-27", "postal_code": "0978585", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0978510','{"jis": "01214", "kana": "ワツカナイネンキンジムシヨ", "name": "稚内年金事務所", "prefecture": "北海道", "city": "稚内市", "neighborhood": "末広", "banchi": "4丁目1-28", "postal_code": "0978510", "old_code": "097  ", "post_office": "稚内", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ホッカイドウ", "city_kana": "ワッカナイシ", "neighborhood_kana": "スエヒロ", "alternates": []}');
 INSERT INTO office_data VALUES('0790197','{"jis": "01215", "kana": "センシユウダイガクホツカイドウタンキダイガク", "name": "専修大学北海道短期大学", "prefecture": "北海道", "city": "美唄市", "neighborhood": "字美唄", "banchi": "1610-1", "postal_code": "0790197", "old_code": "072  ", "post_office": "美唄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -122716,15 +122766,15 @@
 INSERT INTO office_data VALUES('9988501','{"jis": "06204", "kana": "ドクリツギヨウセイホウジン ヤマガタケン・サカタシビヨウインキコウ ニホンカイソウゴウビヨウイン", "name": "独立行政法人　山形県・酒田市病院機構　日本海総合病院", "prefecture": "山形県", "city": "酒田市", "neighborhood": "あきほ町", "banchi": "30", "postal_code": "9988501", "old_code": "998  ", "post_office": "酒田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サカタシ", "neighborhood_kana": "アキホチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9988585','{"jis": "06204", "kana": "ニホンカイソウゴウビヨウイン サカタイリヨウセンタ-", "name": "日本海総合病院　酒田医療センター", "prefecture": "山形県", "city": "酒田市", "neighborhood": "千石町", "banchi": "2丁目3-20", "postal_code": "9988585", "old_code": "998  ", "post_office": "酒田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サカタシ", "neighborhood_kana": "センゴクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9980194','{"jis": "06204", "kana": "トウホクエプソン カブシキガイシヤ", "name": "東北エプソン　株式会社", "prefecture": "山形県", "city": "酒田市", "neighborhood": "大字十里塚", "banchi": "字村東山166-3", "postal_code": "9980194", "old_code": "99801", "post_office": "袖浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9980192','{"jis": "06204", "kana": "トウホクニホンハム カブシキガイシヤ", "name": "東北日本ハム　株式会社", "prefecture": "山形県", "city": "酒田市", "neighborhood": "広栄町", "banchi": "3丁目1", "postal_code": "9980192", "old_code": "99801", "post_office": "袖浦", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サカタシ", "neighborhood_kana": "コウエイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9988611','{"jis": "06204", "kana": "マエダセイカン カブシキガイシヤ", "name": "前田製管　株式会社", "prefecture": "山形県", "city": "酒田市", "neighborhood": "上本町", "banchi": "6-7(酒田郵便局私書箱第4号)", "postal_code": "9988611", "old_code": "99891", "post_office": "酒田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サカタシ", "neighborhood_kana": "カミホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9998292','{"jis": "06204", "kana": "サカタシヤクシヨ ヤワタソウゴウシシヨ", "name": "酒田市役所　八幡総合支所", "prefecture": "山形県", "city": "酒田市", "neighborhood": "観音寺", "banchi": "字寺ノ下41", "postal_code": "9998292", "old_code": "99982", "post_office": "酒田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サカタシ", "neighborhood_kana": "カンノンジ", "alternates": []}');
 INSERT INTO office_data VALUES('9968501','{"jis": "06205", "kana": "シンジヨウシヤクシヨ", "name": "新庄市役所", "prefecture": "山形県", "city": "新庄市", "neighborhood": "沖の町", "banchi": "10-37", "postal_code": "9968501", "old_code": "996  ", "post_office": "新庄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "シンジョウシ", "neighborhood_kana": "オキノマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9968585','{"jis": "06205", "kana": "ヤマガタケンリツ シンジヨウビヨウイン", "name": "山形県立　新庄病院", "prefecture": "山形県", "city": "新庄市", "neighborhood": "金沢", "banchi": "720番地の1", "postal_code": "9968585", "old_code": "996  ", "post_office": "新庄", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマガタケン", "city_kana": "シンジョウシ", "neighborhood_kana": "カナザワ", "alternates": []}');
+INSERT INTO office_data VALUES('9968585','{"jis": "06205", "kana": "ヤマガタケンリツ シンジヨウビヨウイン", "name": "山形県立　新庄病院", "prefecture": "山形県", "city": "新庄市", "neighborhood": "金沢", "banchi": "720番地の1", "postal_code": "9968585", "old_code": "996  ", "post_office": "新庄", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "シンジョウシ", "neighborhood_kana": "カナザワ", "alternates": []}');
 INSERT INTO office_data VALUES('9968602','{"jis": "06205", "kana": "サイホクセイミツ カブシキガイシヤ", "name": "最北精密　株式会社", "prefecture": "山形県", "city": "新庄市", "neighborhood": "金沢", "banchi": "1125(新庄郵便局私書箱第1号)", "postal_code": "9968602", "old_code": "99691", "post_office": "新庄", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "シンジョウシ", "neighborhood_kana": "カナザワ", "alternates": []}');
 INSERT INTO office_data VALUES('9918505','{"jis": "06206", "kana": "サガエコウキヨウシヨクギヨウアンテイジヨ", "name": "寒河江公共職業安定所", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "大字西根", "banchi": "字石川西340", "postal_code": "9918505", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9918555','{"jis": "06206", "kana": "サガエシシヨウコウカイ", "name": "寒河江市商工会", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "中央", "banchi": "1丁目8-38", "postal_code": "9918555", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サガエシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('9918508','{"jis": "06206", "kana": "サガエシリツビヨウイン", "name": "寒河江市立病院", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "大字寒河江", "banchi": "字塩水80", "postal_code": "9918508", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9918585','{"jis": "06206", "kana": "サガエニシムラヤマノウギヨウキヨウドウクミアイ", "name": "さがえ西村山農業協同組合", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "中央工業団地", "banchi": "75", "postal_code": "9918585", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サガエシ", "neighborhood_kana": "チュウオウコウギョウダンチ", "alternates": []}');
 INSERT INTO office_data VALUES('9918521','{"jis": "06206", "kana": "ニシムラヤマフクシジムシヨ", "name": "西村山福祉事務所", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "大字西根", "banchi": "字石川西355", "postal_code": "9918521", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9918610','{"jis": "06206", "kana": "ニツトウベスト カブシキガイシヤ", "name": "日東ベスト　株式会社", "prefecture": "山形県", "city": "寒河江市", "neighborhood": "幸町", "banchi": "4-27", "postal_code": "9918610", "old_code": "991  ", "post_office": "寒河江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマガタケン", "city_kana": "サガエシ", "neighborhood_kana": "サイワイチョウ", "alternates": []}');
@@ -123239,19 +123289,22 @@
 INSERT INTO office_data VALUES('3058563','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバチユウオウダイサンジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば中央第３事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "梅園", "banchi": "1丁目1-1中央第3", "postal_code": "3058563", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ウメゾノ", "alternates": []}');
 INSERT INTO office_data VALUES('3058567','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバチユウオウダイナナジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば中央第７事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "東", "banchi": "1丁目1-1中央第7", "postal_code": "3058567", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3058568','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバチユウオウダイニジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば中央第２事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "梅園", "banchi": "1丁目1-1中央第2", "postal_code": "3058568", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ウメゾノ", "alternates": []}');
 INSERT INTO office_data VALUES('3058566','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバチユウオウダイロクジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば中央第６事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "東", "banchi": "1丁目1-1中央第6", "postal_code": "3058566", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3058569','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバニシジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば西事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "小野川", "banchi": "16-1", "postal_code": "3058569", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "オノガワ", "alternates": []}');
 INSERT INTO office_data VALUES('3058564','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン サンギヨウギジユツソウゴウケンキユウジヨ ツクバヒガシジギヨウシヨ", "name": "国立研究開発法人　産業技術総合研究所　つくば東事業所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "並木", "banchi": "1丁目2-1", "postal_code": "3058564", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ナミキ", "alternates": []}');
 INSERT INTO office_data VALUES('3058517','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ", "name": "国立研究開発法人　農業・食品産業技術総合研究機構", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "3-1-1", "postal_code": "3058517", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
-INSERT INTO office_data VALUES('3058605','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ カジユチヤギヨウケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　果樹茶業研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "藤本", "banchi": "2-1", "postal_code": "3058605", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "フジモト", "alternates": []}');
-INSERT INTO office_data VALUES('3058518','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ジセダイサクモツカイハツケンキユウセンタ-", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　次世代作物開発研究センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2-1-2", "postal_code": "3058518", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
-INSERT INTO office_data VALUES('3058634','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ セイブツキノウリヨウケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　生物機能利用研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "大わし", "banchi": "1-2", "postal_code": "3058634", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "オオワシ", "alternates": []}');
+INSERT INTO office_data VALUES('3058605','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ カジユチヤギヨウケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　果樹茶業研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "藤本", "banchi": "2-1", "postal_code": "3058605", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "フジモト", "alternates": []}');
+INSERT INTO office_data VALUES('3058602','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ キバンギジユツケンキユウホンブイデンシゲンケンキユウセンタ-", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　基盤技術研究本部遺伝資源研究センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-2", "postal_code": "3058602", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
+INSERT INTO office_data VALUES('3058518','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ サクモツケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　作物研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-2", "postal_code": "3058518", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
+INSERT INTO office_data VALUES('3058642','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ シヨクヒンケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　食品研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-12", "postal_code": "3058642", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
+INSERT INTO office_data VALUES('3058634','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ セイブツキノウリヨウケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　生物機能利用研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "大わし", "banchi": "1-2", "postal_code": "3058634", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "オオワシ", "alternates": []}');
 INSERT INTO office_data VALUES('3058666','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ チユウオウノウギヨウケンキユウセンタ-", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　中央農業研究センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2-1-18", "postal_code": "3058666", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058604','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ノウギヨウカンキヨウヘンドウケンキユウセンタ-", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　農業環境変動研究センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "三丁目1番地3", "postal_code": "3058604", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
+INSERT INTO office_data VALUES('3058609','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ノウソンコウガクケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　農村工学研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-6", "postal_code": "3058609", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058519','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ヤサイカキケンキユウブモン", "name": "国立研究開発法人　農業・食品産業技術総合研究機構　野菜花き研究部門", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "3-1-1", "postal_code": "3058519", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058560','{"jis": "08220", "kana": "コクリツケンキユウカイハツホウジンサンギヨウギジユツソウゴウケンキユウシヨツクバチユウオウダイイチジギヨウシヨ(ツクバホンブ・ジヨウホウギジユツキヨウドウケンキユウトウ)", "name": "国立研究開発法人　産業技術総合研究所　つくば中央第１事業所　（つくば本部・情報技術共同研究棟）", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "梅園", "banchi": "1丁目1-1中央第1", "postal_code": "3058560", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ウメゾノ", "alternates": []}');
 INSERT INTO office_data VALUES('3058520','{"jis": "08220", "kana": "コクリツダイガクホウジン ツクバギジユツダイガク アマクボキヤンパス", "name": "国立大学法人　筑波技術大学　天久保キャンパス", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天久保", "banchi": "4丁目3-15", "postal_code": "3058520", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "アマクボ", "alternates": []}');
 INSERT INTO office_data VALUES('3058521','{"jis": "08220", "kana": "コクリツダイガクホウジン ツクバギジユツダイガク カスガキヤンパス", "name": "国立大学法人　筑波技術大学　春日キャンパス", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "春日", "banchi": "4丁目12-7", "postal_code": "3058521", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カスガ", "alternates": []}');
 INSERT INTO office_data VALUES('3058515','{"jis": "08220", "kana": "セキシヨウシヨウジ カブシキカイシヤ", "name": "関彰商事　株式会社", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "東新井", "banchi": "12-2", "postal_code": "3058515", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ヒガシアライ", "alternates": []}');
 INSERT INTO office_data VALUES('3058555','{"jis": "08220", "kana": "ツクバシヤクシヨ", "name": "つくば市役所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "研究学園", "banchi": "一丁目1番地1", "postal_code": "3058555", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ケンキュウガクエン", "alternates": []}');
 INSERT INTO office_data VALUES('3058575','{"jis": "08220", "kana": "ツクバダイガク イガクセンモンガクグン", "name": "筑波大学　医学専門学群", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天王台", "banchi": "1-1-1", "postal_code": "3058575", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "テンノウダイ", "alternates": []}');
@@ -123260,17 +123313,14 @@
 INSERT INTO office_data VALUES('3058573','{"jis": "08220", "kana": "ツクバダイガク ダイサンガクグン システムジヨウホウ", "name": "筑波大学　第三学群　システム情報", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天王台", "banchi": "1-1-1", "postal_code": "3058573", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "テンノウダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058572','{"jis": "08220", "kana": "ツクバダイガク ダイニガクグン ニンゲン", "name": "筑波大学　第二学群　人間", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天王台", "banchi": "1-1-1", "postal_code": "3058572", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "テンノウダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058550','{"jis": "08220", "kana": "ツクバダイガク トシヨカンジヨウホウメデイア", "name": "筑波大学　図書館情報メディア", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "春日", "banchi": "1-2", "postal_code": "3058550", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カスガ", "alternates": []}');
 INSERT INTO office_data VALUES('3058577','{"jis": "08220", "kana": "ツクバダイガク(ジムキヨク・チユウオウトシヨカン)", "name": "筑波大学（事務局・中央図書館）", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天王台", "banchi": "1-1-1", "postal_code": "3058577", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "テンノウダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058576','{"jis": "08220", "kana": "ツクバダイガクフゾクビヨウイン", "name": "筑波大学付属病院", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "天久保", "banchi": "2-1-1", "postal_code": "3058576", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "アマクボ", "alternates": []}');
 INSERT INTO office_data VALUES('3058505','{"jis": "08220", "kana": "ドクリツギヨウセイホウジン ウチユウコウクウケンキユウカイハツキコウ ツクバウチユウセンタ-", "name": "独立行政法人　宇宙航空研究開発機構　筑波宇宙センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "千現", "banchi": "2-1-1", "postal_code": "3058505", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "センゲン", "alternates": []}');
 INSERT INTO office_data VALUES('3058506','{"jis": "08220", "kana": "ドクリツギヨウセイホウジン コクリツカンキヨウケンキユウジヨ", "name": "独立行政法人　国立環境研究所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "小野川", "banchi": "16-2", "postal_code": "3058506", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "オノガワ", "alternates": []}');
-INSERT INTO office_data VALUES('3058642','{"jis": "08220", "kana": "ドクリツギヨウセイホウジン シヨクヒンソウゴウケンキユウジヨ", "name": "独立行政法人　食品総合研究所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-2(筑波農林研究団地内郵便局私書箱第11号)", "postal_code": "3058642", "old_code": "305  ", "post_office": "筑波学園", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
-INSERT INTO office_data VALUES('3058609','{"jis": "08220", "kana": "ドクリツギヨウセイホウジン ノウギヨウ・シヨクヒンサンギヨウギジユツソウゴウケンキユウキコウ ノウソンコウガクケンキユウシヨ", "name": "独立行政法人　農業・食品産業技術総合研究機構　農村工学研究所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-6", "postal_code": "3058609", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
-INSERT INTO office_data VALUES('3058602','{"jis": "08220", "kana": "ドクリツギヨウセイホウジン ノウギヨウセイブツシゲンケンキユウジヨ", "name": "独立行政法人　農業生物資源研究所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1-2(筑波農林研究団地内郵便局私書箱第12号)", "postal_code": "3058602", "old_code": "305  ", "post_office": "筑波学園", "type": "box", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058501','{"jis": "08220", "kana": "ニホンデンキ カブシキガイシヤ ツクバケンキユウジヨ", "name": "日本電気　株式会社　筑波研究所", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "御幸が丘", "banchi": "34番地", "postal_code": "3058501", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "ミユキガオカ", "alternates": []}');
 INSERT INTO office_data VALUES('3058601','{"jis": "08220", "kana": "ノウリンスイサンギジユツカイギジムキヨク ツクバサンガクレンケイシエンセンタ-", "name": "農林水産技術会議事務局　筑波産学連携支援センター", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "観音台", "banchi": "2丁目1番9", "postal_code": "3058601", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "カンノンダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3058502','{"jis": "08220", "kana": "メイケイガクエンチユウガツコウコウトウガツコウ", "name": "茗溪学園中学校高等学校", "prefecture": "茨城県", "city": "つくば市", "neighborhood": "稲荷前", "banchi": "1-1", "postal_code": "3058502", "old_code": "305  ", "post_office": "筑波学園", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ツクバシ", "neighborhood_kana": "イナリマエ", "alternates": []}');
 INSERT INTO office_data VALUES('3128508','{"jis": "08221", "kana": "イバラキコウギヨウコウトウセンモンガツコウ", "name": "茨城工業高等専門学校", "prefecture": "茨城県", "city": "ひたちなか市", "neighborhood": "大字中根", "banchi": "866", "postal_code": "3128508", "old_code": "312  ", "post_office": "ひたちなか", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3128510','{"jis": "08221", "kana": "カブシキガイシヤ ジヨイフルホンダ ニユ-ポ-トヒタチナカテン", "name": "株式会社　ジョイフル本田　ニューポートひたちなか店", "prefecture": "茨城県", "city": "ひたちなか市", "neighborhood": "新光町", "banchi": "34-1", "postal_code": "3128510", "old_code": "312  ", "post_office": "ひたちなか", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イバラキケン", "city_kana": "ヒタチナカシ", "neighborhood_kana": "シンコウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3128504','{"jis": "08221", "kana": "カブシキガイシヤ ヒタチハイテクノロジ-ズ", "name": "株式会社　日立ハイテクノロジーズ", "prefecture": "茨城県", "city": "ひたちなか市", "neighborhood": "大字市毛", "banchi": "882番地", "postal_code": "3128504", "old_code": "312  ", "post_office": "ひたちなか", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3128507','{"jis": "08221", "kana": "カブシキガイシヤ ヒタチパワ-ソリユ-シヨンズ カツタジギヨウシヨ", "name": "株式会社　日立パワーソリューションズ　勝田事業所", "prefecture": "茨城県", "city": "ひたちなか市", "neighborhood": "大字堀口", "banchi": "832番地の2", "postal_code": "3128507", "old_code": "312  ", "post_office": "ひたちなか", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -123943,15 +123993,15 @@
 INSERT INTO office_data VALUES('3318540','{"jis": "11102", "kana": "ユアサシヨウジ カブシキガイシヤ キタカントウシシヤ", "name": "ユアサ商事　株式会社　北関東支社", "prefecture": "埼玉県", "city": "さいたま市北区", "neighborhood": "宮原町", "banchi": "4-7-5", "postal_code": "3318540", "old_code": "331  ", "post_office": "大宮西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシキタク", "neighborhood_kana": "ミヤハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3318550','{"jis": "11102", "kana": "リクジヨウジエイタイ オオミヤチユウトンチ", "name": "陸上自衛隊　大宮駐屯地", "prefecture": "埼玉県", "city": "さいたま市北区", "neighborhood": "日進町", "banchi": "1丁目40-7", "postal_code": "3318550", "old_code": "331  ", "post_office": "大宮西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシキタク", "neighborhood_kana": "ニッシンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308688','{"jis": "11103", "kana": "アクサソンガイホケン カブシキカイシヤ", "name": "アクサ損害保険　株式会社", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "土手町", "banchi": "1丁目2JA共済埼玉ビル", "postal_code": "3308688", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ドテチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308505','{"jis": "11103", "kana": "エヌテイ-テイ- オオミヤシテン", "name": "ＮＴＴ　大宮支店", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "下町", "banchi": "2丁目61", "postal_code": "3308505", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "シモチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308589','{"jis": "11103", "kana": "オオミヤラク-ン", "name": "大宮ラクーン", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "宮町", "banchi": "1-60", "postal_code": "3308589", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3309559','{"jis": "11103", "kana": "カタクラコウギヨウ カブシキガイシヤ コク-ンシテイ", "name": "片倉工業　株式会社　コクーンシティ", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "吉敷町", "banchi": "4-263-1", "postal_code": "3309559", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "キシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308579','{"jis": "11103", "kana": "カブシキガイシヤ エフエムナツクフアイブ", "name": "株式会社　ＦＭＮＡＣＫ５", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "錦町", "banchi": "682-2JACK大宮11F", "postal_code": "3308579", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('3308564','{"jis": "11103", "kana": "カブシキガイシヤ カンデンコウ キタカントウ・ホクシンエツエイギヨウホンブ", "name": "株式会社　関電工　北関東・北信越営業本部", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "桜木町", "banchi": "1-195-1大宮ソラミチKOZ8階", "postal_code": "3308564", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('3308564','{"jis": "11103", "kana": "カブシキガイシヤ カンデンコウ キタカントウ・ホクシンエツエイギヨウホンブ", "name": "株式会社　関電工　北関東・北信越営業本部", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "桜木町", "banchi": "1-195-1大宮ソラミチKOZ8階", "postal_code": "3308564", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3309520','{"jis": "11103", "kana": "カブシキガイシヤ シマムラ", "name": "株式会社　しまむら", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "北袋町", "banchi": "1丁目602番1号", "postal_code": "3309520", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "キタブクロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308511','{"jis": "11103", "kana": "カブシキガイシヤ タカシマヤ オオミヤテン", "name": "株式会社　高島屋　大宮店", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "大門町", "banchi": "1丁目32", "postal_code": "3308511", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ダイモンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308547','{"jis": "11103", "kana": "カブシキガイシヤ ニツポンセイサクキンユウコウコ サイタマシテン コクミンセイカツジギヨウ", "name": "株式会社　日本政策金融公庫　さいたま支店　国民生活事業", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "宮町", "banchi": "1丁目109-1大宮宮町ビル4F", "postal_code": "3308547", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3309503','{"jis": "11103", "kana": "カブシキガイシヤ フジツウマ-ケテイング", "name": "株式会社　富士通マーケティング", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "桜木町", "banchi": "1丁目11-20大宮JPビルディング", "postal_code": "3309503", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308581','{"jis": "11103", "kana": "カブシキガイシヤ フジヤクヒン", "name": "株式会社　富士薬品", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "桜木町", "banchi": "2丁目292-1", "postal_code": "3308581", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3309621','{"jis": "11103", "kana": "カブシキガイシヤ ロフト オオミヤロフト", "name": "株式会社　ロフト　大宮ロフト", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "宮町", "banchi": "1丁目60", "postal_code": "3309621", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "ミヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3308548','{"jis": "11103", "kana": "ガツコウホウジン コクサイガクイン コクサイガクインサイタマタンキダイガク", "name": "学校法人　国際学院　国際学院埼玉短期大学", "prefecture": "埼玉県", "city": "さいたま市大宮区", "neighborhood": "吉敷町", "banchi": "2丁目5番地", "postal_code": "3308548", "old_code": "330  ", "post_office": "さいたま新都心", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サイタマシオオミヤク", "neighborhood_kana": "キシキチョウ", "alternates": []}');
@@ -124296,14 +124346,15 @@
 INSERT INTO office_data VALUES('3448680','{"jis": "11214", "kana": "カントウシンエツコクゼイキヨク インボイストウロクセンタ-", "name": "関東信越国税局　インボイス登録センター", "prefecture": "埼玉県", "city": "春日部市", "neighborhood": "大沼", "banchi": "2丁目12番地1", "postal_code": "3448680", "old_code": "344  ", "post_office": "春日部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "カスカベシ", "neighborhood_kana": "オオヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3448555','{"jis": "11214", "kana": "サイタマケンカスカベケンゼイジムシヨ", "name": "埼玉県春日部県税事務所", "prefecture": "埼玉県", "city": "春日部市", "neighborhood": "大沼", "banchi": "1丁目76", "postal_code": "3448555", "old_code": "344  ", "post_office": "春日部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "カスカベシ", "neighborhood_kana": "オオヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3448508','{"jis": "11214", "kana": "サイタマケンシンヨウホシヨウキヨウカイ カスカベシテン", "name": "埼玉県信用保証協会　春日部支店", "prefecture": "埼玉県", "city": "春日部市", "neighborhood": "南", "banchi": "1丁目1番7号埼玉県東部地域振興ふれあい拠点施設5階", "postal_code": "3448508", "old_code": "344  ", "post_office": "春日部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "カスカベシ", "neighborhood_kana": "ミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('3448533','{"jis": "11214", "kana": "セイブ カスカベテン", "name": "西武　春日部店", "prefecture": "埼玉県", "city": "春日部市", "neighborhood": "粕壁東", "banchi": "2丁目5番1号", "postal_code": "3448533", "old_code": "344  ", "post_office": "春日部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "カスカベシ", "neighborhood_kana": "カスカベヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3501385','{"jis": "11215", "kana": "アベコウギヨウ カブシキガイシヤ", "name": "阿部興業　株式会社", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "新狭山", "banchi": "1-1-11", "postal_code": "3501385", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "シンサヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('3501386','{"jis": "11215", "kana": "アマゾン サヤマエフシ- ニユウコカカリ", "name": "アマゾン　狭山ＦＣ　入庫係", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "青柳", "banchi": "915-1", "postal_code": "3501386", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "アオヤギ", "alternates": []}');
 INSERT INTO office_data VALUES('3501389','{"jis": "11215", "kana": "アマゾンサヤマヒダカエフシ-", "name": "アマゾン狭山日高ＦＣ", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "広瀬台", "banchi": "4丁目5番", "postal_code": "3501389", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "ヒロセダイ", "alternates": []}');
+INSERT INTO office_data VALUES('3501383','{"jis": "11215", "kana": "アマゾンサヤマヒロセダイエフシ-", "name": "アマゾン狭山広瀬台ＦＣ", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "広瀬台", "banchi": "2丁目4-3", "postal_code": "3501383", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "ヒロセダイ", "alternates": []}');
 INSERT INTO office_data VALUES('3501395','{"jis": "11215", "kana": "カブシキガイシヤ サギノミヤセイサクシヨ サヤマジギヨウシヨ", "name": "株式会社　鷺宮製作所　狭山事業所", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "笹井", "banchi": "535", "postal_code": "3501395", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "ササイ", "alternates": []}');
 INSERT INTO office_data VALUES('3501380','{"jis": "11215", "kana": "サヤマシヤクシヨ", "name": "狭山市役所", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "入間川", "banchi": "1丁目23-5", "postal_code": "3501380", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "イルマガワ", "alternates": []}');
 INSERT INTO office_data VALUES('3501388','{"jis": "11215", "kana": "トウアデイ-ケ-ケ- カブシキカイシヤ サヤマテクニカルセンタ-", "name": "東亜ディーケーケー　株式会社　狭山テクニカルセンター", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "北入曽", "banchi": "613", "postal_code": "3501388", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "キタイリソ", "alternates": []}');
 INSERT INTO office_data VALUES('3501398','{"jis": "11215", "kana": "トウキヨウカセイダイガク サヤマコウシヤ", "name": "東京家政大学　狭山校舎", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "稲荷山", "banchi": "2丁目15-1", "postal_code": "3501398", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "イナリヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('3501392','{"jis": "11215", "kana": "ホンダギケンコウギヨウ カブシキガイシヤ サイタマセイサクジヨ", "name": "本田技研工業　株式会社　埼玉製作所", "prefecture": "埼玉県", "city": "狭山市", "neighborhood": "新狭山", "banchi": "1丁目10-1", "postal_code": "3501392", "old_code": "35013", "post_office": "狭山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "サヤマシ", "neighborhood_kana": "シンサヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('3488508','{"jis": "11216", "kana": "アケボノブレ-キコウギヨウ カブシキガイシヤ", "name": "曙ブレーキ工業　株式会社", "prefecture": "埼玉県", "city": "羽生市", "neighborhood": "東", "banchi": "5-4-71", "postal_code": "3488508", "old_code": "348  ", "post_office": "羽生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "ハニュウシ", "neighborhood_kana": "ヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('3488501','{"jis": "11216", "kana": "アケボノブレ-キコウギヨウ カブシキガイシヤ カントウエイギヨウシヨ", "name": "曙ブレーキ工業　株式会社　関東営業所", "prefecture": "埼玉県", "city": "羽生市", "neighborhood": "東", "banchi": "5-4-71", "postal_code": "3488501", "old_code": "348  ", "post_office": "羽生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "ハニュウシ", "neighborhood_kana": "ヒガシ", "alternates": []}');
@@ -124461,15 +124512,15 @@
 INSERT INTO office_data VALUES('3468516','{"jis": "11232", "kana": "イト-ヨ-カドウ クキアイデイ-シ-(テイ-シ-)", "name": "イトーヨーカ堂　久喜ＩＤＣ（ＴＣ）", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "清久町", "banchi": "1-10MFLP1階", "postal_code": "3468516", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "キヨクチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3468501','{"jis": "11232", "kana": "クキシヤクシヨ", "name": "久喜市役所", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "大字下早見", "banchi": "85-3", "postal_code": "3468501", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3468530','{"jis": "11232", "kana": "サイタマケンコウセイノウギヨウキヨウドウクミアイレンゴウカイ クキソウゴウビヨウイン", "name": "埼玉県厚生農業協同組合連合会　久喜総合病院", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "上早見", "banchi": "418番地1", "postal_code": "3468530", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "カミハヤミ", "alternates": []}');
 INSERT INTO office_data VALUES('3468506','{"jis": "11232", "kana": "サイタマケンリツクキトシヨカン", "name": "埼玉県立久喜図書館", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "大字下早見", "banchi": "85-5", "postal_code": "3468506", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3468524','{"jis": "11232", "kana": "ニホンシンゴウ (カブ)", "name": "日本信号　（株）", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "大字江面", "banchi": "1836番地1号", "postal_code": "3468524", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3468685','{"jis": "11232", "kana": "ベネツセコ-ポレ-シヨン", "name": "ベネッセコーポレーション", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "河原井町", "banchi": "7", "postal_code": "3468685", "old_code": "346  ", "post_office": "久喜", "type": "box", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "カワライチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3468540','{"jis": "11232", "kana": "ベネツセコ-ポレ-シヨン (カブ)", "name": "ベネッセコーポレーション　（株）", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "河原井町", "banchi": "7", "postal_code": "3468540", "old_code": "346  ", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "カワライチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('3460181','{"jis": "11232", "kana": "カブシキカイシヤ ニチデン トウブブツリユウセンタ-", "name": "株式会社　日伝　東部物流センター", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町三箇", "banchi": "5番5", "postal_code": "3460181", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": true, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウサンガ", "alternates": []}');
+INSERT INTO office_data VALUES('3460181','{"jis": "11232", "kana": "カブシキカイシヤ ニチデン トウブブツリユウセンタ-", "name": "株式会社　日伝　東部物流センター", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町三箇", "banchi": "5番5", "postal_code": "3460181", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウサンガ", "alternates": []}');
 INSERT INTO office_data VALUES('3460198','{"jis": "11232", "kana": "カブシキガイシヤ エヌエスケ-マシナリ-", "name": "株式会社　ＮＳＫマシナリー", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町昭和沼", "banchi": "5", "postal_code": "3460198", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウショウワヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3460194','{"jis": "11232", "kana": "カブシキガイシヤ エフテツク", "name": "株式会社　エフテック", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町昭和沼", "banchi": "19", "postal_code": "3460194", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウショウワヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3460192','{"jis": "11232", "kana": "クキシ シヨウブソウゴウシシヨ", "name": "久喜市　菖蒲総合支所", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町新堀", "banchi": "38番地", "postal_code": "3460192", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウニイボリ", "alternates": []}');
 INSERT INTO office_data VALUES('3460193','{"jis": "11232", "kana": "ニホンチユウテツカン カブシキガイシヤ", "name": "日本鋳鉄管　株式会社", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町昭和沼", "banchi": "1", "postal_code": "3460193", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウショウワヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3460196','{"jis": "11232", "kana": "ニホンマタイ カブシキガイシヤ サイタマコウジヨウ", "name": "日本マタイ　株式会社　埼玉工場", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町昭和沼", "banchi": "22", "postal_code": "3460196", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウショウワヌマ", "alternates": []}');
 INSERT INTO office_data VALUES('3460195','{"jis": "11232", "kana": "モラ-ジユシヨウブ", "name": "モラージュ菖蒲", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町菖蒲", "banchi": "字伊勢浦3555番地", "postal_code": "3460195", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウショウブ", "alternates": []}');
 INSERT INTO office_data VALUES('3460183','{"jis": "11232", "kana": "ユニ-グル-プカントウキタブツリユウセンタ-", "name": "ユニーグループ関東北物流センター", "prefecture": "埼玉県", "city": "久喜市", "neighborhood": "菖蒲町三箇", "banchi": "字金芳面6201-3", "postal_code": "3460183", "old_code": "34601", "post_office": "久喜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "サイタマケン", "city_kana": "クキシ", "neighborhood_kana": "ショウブチョウサンガ", "alternates": []}');
@@ -124745,15 +124796,15 @@
 INSERT INTO office_data VALUES('2648530','{"jis": "12104", "kana": "ミツワダイソウゴウビヨウイン", "name": "みつわ台総合病院", "prefecture": "千葉県", "city": "千葉市若葉区", "neighborhood": "若松町", "banchi": "531-486", "postal_code": "2648530", "old_code": "264  ", "post_office": "若葉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシワカバク", "neighborhood_kana": "ワカマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2648501','{"jis": "12104", "kana": "リクジヨウジエイタイ シモシヅチユウトンチ", "name": "陸上自衛隊　下志津駐屯地", "prefecture": "千葉県", "city": "千葉市若葉区", "neighborhood": "若松町", "banchi": "902", "postal_code": "2648501", "old_code": "264  ", "post_office": "若葉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシワカバク", "neighborhood_kana": "ワカマツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2648733','{"jis": "12104", "kana": "ワカバクヤクシヨ", "name": "若葉区役所", "prefecture": "千葉県", "city": "千葉市若葉区", "neighborhood": "桜木町", "banchi": "567-1", "postal_code": "2648733", "old_code": "264  ", "post_office": "若葉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2658501','{"jis": "12104", "kana": "トウキヨウジヨウホウダイガク", "name": "東京情報大学", "prefecture": "千葉県", "city": "千葉市若葉区", "neighborhood": "御成台", "banchi": "4-1", "postal_code": "2658501", "old_code": "265  ", "post_office": "若葉", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシワカバク", "neighborhood_kana": "オナリダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2668550','{"jis": "12105", "kana": "チバシ ミドリホケンフクシセンタ-", "name": "千葉市　緑保健福祉センター", "prefecture": "千葉県", "city": "千葉市緑区", "neighborhood": "鎌取町", "banchi": "226-1", "postal_code": "2668550", "old_code": "266  ", "post_office": "千葉緑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミドリク", "neighborhood_kana": "カマトリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2668733','{"jis": "12105", "kana": "チバシミドリクヤクシヨ", "name": "千葉市緑区役所", "prefecture": "千葉県", "city": "千葉市緑区", "neighborhood": "おゆみ野", "banchi": "3丁目15番地3号", "postal_code": "2668733", "old_code": "266  ", "post_office": "千葉緑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミドリク", "neighborhood_kana": "オユミノ", "alternates": []}');
 INSERT INTO office_data VALUES('2618575','{"jis": "12106", "kana": "(カブ) ニツサンフイナンシヤルサ-ビス", "name": "（株）　日産フィナンシャルサービス", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "中瀬", "banchi": "2丁目6ワールドビジネスガーデンマリブウエスト13F", "postal_code": "2618575", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "ナカセ", "alternates": []}');
-INSERT INTO office_data VALUES('2618528','{"jis": "12106", "kana": "アマゾンチバミナトエフシ-", "name": "アマゾン千葉みなとＦＣ", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "新港", "banchi": "68-1", "postal_code": "2618528", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "シンミナト", "alternates": []}');
+INSERT INTO office_data VALUES('2618528','{"jis": "12106", "kana": "アマゾンチバミナトエフシ-", "name": "アマゾン千葉みなとＦＣ", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "新港", "banchi": "68-1", "postal_code": "2618528", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "シンミナト", "alternates": []}');
 INSERT INTO office_data VALUES('2618515','{"jis": "12106", "kana": "イオン カブシキガイシヤ", "name": "イオン　株式会社", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "中瀬", "banchi": "1丁目5-1", "postal_code": "2618515", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "ナカセ", "alternates": []}');
 INSERT INTO office_data VALUES('2618541','{"jis": "12106", "kana": "イオンコンパス (カ) オペレ-シヨンセンタ- ハガキジムキヨク", "name": "イオンコンパス　（株）　オペレーションセンター　ハガキ事務局", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "中瀬", "banchi": "2-6-1WBGマリブイースト5F", "postal_code": "2618541", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "ナカセ", "alternates": []}');
 INSERT INTO office_data VALUES('2618539','{"jis": "12106", "kana": "イオンモ-ル カブシキガイシヤ", "name": "イオンモール　株式会社", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "中瀬", "banchi": "一丁目5番地1", "postal_code": "2618539", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "ナカセ", "alternates": []}');
 INSERT INTO office_data VALUES('2618535','{"jis": "12106", "kana": "イオンモ-ル マクハリシントシン", "name": "イオンモール　幕張新都心", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "豊砂", "banchi": "1-1", "postal_code": "2618535", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "トヨスナ", "alternates": []}');
 INSERT INTO office_data VALUES('2618503','{"jis": "12106", "kana": "イオンリテ-ル カブシキガイシヤ イナゲカイガンジムシヨ", "name": "イオンリテール　株式会社　稲毛海岸事務所", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "高洲", "banchi": "3-13-2", "postal_code": "2618503", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "タカス", "alternates": []}');
 INSERT INTO office_data VALUES('2618513','{"jis": "12106", "kana": "イオンリテ-ル カブシキガイシヤ ジヤスコマリンピアテン", "name": "イオンリテール　株式会社　ジャスコマリンピア店", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "高洲", "banchi": "3-13-1", "postal_code": "2618513", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "タカス", "alternates": []}');
 INSERT INTO office_data VALUES('2618504','{"jis": "12106", "kana": "カブシキガイシヤ イオンフアンタジ-", "name": "株式会社　イオンファンタジー", "prefecture": "千葉県", "city": "千葉市美浜区", "neighborhood": "中瀬", "banchi": "1-5-1", "postal_code": "2618504", "old_code": "261  ", "post_office": "美浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "チバシミハマク", "neighborhood_kana": "ナカセ", "alternates": []}');
@@ -125130,15 +125181,15 @@
 INSERT INTO office_data VALUES('2798521','{"jis": "12227", "kana": "カブシキガイシヤ マイハマコ-ポレ-シヨン", "name": "株式会社　舞浜コーポレーション", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地1", "postal_code": "2798521", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798553','{"jis": "12227", "kana": "カブシキガイシヤ リ-ガルコ-ポレ-シヨン", "name": "株式会社　リーガルコーポレーション", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "2丁目1-8", "postal_code": "2798553", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
 INSERT INTO office_data VALUES('2798567','{"jis": "12227", "kana": "ガツコウホウジン リヨウトクジダイガク", "name": "学校法人　了徳寺大学", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "明海", "banchi": "23", "postal_code": "2798567", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "アケミ", "alternates": []}');
 INSERT INTO office_data VALUES('2798601','{"jis": "12227", "kana": "サラリコウボウ カブシキガイシヤ", "name": "サラリ工房　株式会社", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "今川", "banchi": "1-11-37", "postal_code": "2798601", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "イマガワ", "alternates": []}');
 INSERT INTO office_data VALUES('2798518','{"jis": "12227", "kana": "シルク・ドウ・ソレイユ シアタ-トウキヨウ", "name": "シルク・ドゥ・ソレイユ　シアター東京", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地50", "postal_code": "2798518", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798522','{"jis": "12227", "kana": "デイズニ-アンバサダ-ホテル", "name": "ディズニーアンバサダーホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "2番地11", "postal_code": "2798522", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798558','{"jis": "12227", "kana": "トウカイダイガクフゾク ウラヤスコウトウガツコウ", "name": "東海大学付属　浦安高等学校", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "東野", "banchi": "3-11-1", "postal_code": "2798558", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒガシノ", "alternates": []}');
-INSERT INTO office_data VALUES('2798526','{"jis": "12227", "kana": "トウキヨウデイズニ-シ-・フアンタジ-スプリングスホテル", "name": "東京ディズニーシー・ファンタジースプリングスホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地2", "postal_code": "2798526", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
+INSERT INTO office_data VALUES('2798526','{"jis": "12227", "kana": "トウキヨウデイズニ-シ-・フアンタジ-スプリングスホテル", "name": "東京ディズニーシー・ファンタジースプリングスホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1番地2", "postal_code": "2798526", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798519','{"jis": "12227", "kana": "トウキヨウデイズニ-シ-・ホテルミラコスタ", "name": "東京ディズニーシー・ホテルミラコスタ", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-13", "postal_code": "2798519", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798505','{"jis": "12227", "kana": "トウキヨウデイズニ-ランドホテル", "name": "東京ディズニーランドホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "29-1", "postal_code": "2798505", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798506','{"jis": "12227", "kana": "トウキヨウデイズニ-リゾ-ト・トイ・スト-リ-ホテル", "name": "東京ディズニーリゾート・トイ・ストーリーホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "舞浜", "banchi": "1-47", "postal_code": "2798506", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "マイハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798530','{"jis": "12227", "kana": "トウキヨウデンリヨク カブシキガイシヤ イチカワウラヤスエイギヨウシヨ", "name": "東京電力　株式会社　市川浦安営業所", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "1", "postal_code": "2798530", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
 INSERT INTO office_data VALUES('2798555','{"jis": "12227", "kana": "トウレ カブシキガイシヤ ダイニホンシヤ", "name": "東レ　株式会社　第２本社", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "美浜", "banchi": "1丁目8-1", "postal_code": "2798555", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ミハマ", "alternates": []}');
 INSERT INTO office_data VALUES('2798588','{"jis": "12227", "kana": "ニホンコ-プキヨウサイセイカツキヨウドウクミアイレンゴウカイ", "name": "日本コープ共済生活協同組合連合会", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "入船", "banchi": "1丁目5-2", "postal_code": "2798588", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "イリフネ", "alternates": []}');
 INSERT INTO office_data VALUES('2798503','{"jis": "12227", "kana": "パ-ムテラスホテル", "name": "パームテラスホテル", "prefecture": "千葉県", "city": "浦安市", "neighborhood": "日の出", "banchi": "7-1-1", "postal_code": "2798503", "old_code": "279  ", "post_office": "浦安", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "ウラヤスシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
@@ -125191,15 +125242,15 @@
 INSERT INTO office_data VALUES('2878555','{"jis": "12236", "kana": "サワラゼイムシヨ", "name": "佐原税務署", "prefecture": "千葉県", "city": "香取市", "neighborhood": "北", "banchi": "1丁目4-1", "postal_code": "2878555", "old_code": "287  ", "post_office": "佐原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カトリシ", "neighborhood_kana": "キタ", "alternates": []}');
 INSERT INTO office_data VALUES('2878503','{"jis": "12236", "kana": "チバケン カトリケンゼイジムシヨ", "name": "千葉県　香取県税事務所", "prefecture": "千葉県", "city": "香取市", "neighborhood": "佐原", "banchi": "イ92-11", "postal_code": "2878503", "old_code": "287  ", "post_office": "佐原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2878502','{"jis": "12236", "kana": "チバケン カトリチイキシンコウジムシヨ", "name": "千葉県　香取地域振興事務所", "prefecture": "千葉県", "city": "香取市", "neighborhood": "佐原", "banchi": "イ92-11", "postal_code": "2878502", "old_code": "287  ", "post_office": "佐原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2878585','{"jis": "12236", "kana": "チバシヤカイホケンジムキヨク サワラジムシヨ", "name": "千葉社会保険事務局　佐原事務所", "prefecture": "千葉県", "city": "香取市", "neighborhood": "佐原", "banchi": "ロ2116-1", "postal_code": "2878585", "old_code": "287  ", "post_office": "佐原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('2890392','{"jis": "12236", "kana": "アタリヤノウエン", "name": "アタリヤ農園", "prefecture": "千葉県", "city": "香取市", "neighborhood": "阿玉川", "banchi": "1103", "postal_code": "2890392", "old_code": "28903", "post_office": "小見川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カトリシ", "neighborhood_kana": "アタマガワ", "alternates": []}');
 INSERT INTO office_data VALUES('2890393','{"jis": "12236", "kana": "カトリシヤクシヨ オミガワシシヨ", "name": "香取市役所　小見川支所", "prefecture": "千葉県", "city": "香取市", "neighborhood": "羽根川", "banchi": "38", "postal_code": "2890393", "old_code": "28903", "post_office": "小見川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カトリシ", "neighborhood_kana": "ハネガワ", "alternates": []}');
 INSERT INTO office_data VALUES('2890492','{"jis": "12236", "kana": "カトリシヤクシヨ ヤマダシシヨ", "name": "香取市役所　山田支所", "prefecture": "千葉県", "city": "香取市", "neighborhood": "仁良", "banchi": "300番地1", "postal_code": "2890492", "old_code": "28904", "post_office": "府馬", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "カトリシ", "neighborhood_kana": "ニラ", "alternates": []}');
-INSERT INTO office_data VALUES('2891297','{"jis": "12237", "kana": "アルバツクマテリアル カブシキガイシヤ", "name": "アルバックマテリアル　株式会社", "prefecture": "千葉県", "city": "山武市", "neighborhood": "横田", "banchi": "516番地", "postal_code": "2891297", "old_code": "28912", "post_office": "日向", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "ヨコタ", "alternates": []}');
+INSERT INTO office_data VALUES('2891297','{"jis": "12237", "kana": "カブシキガイシヤ アルバツク", "name": "株式会社　アルバック", "prefecture": "千葉県", "city": "山武市", "neighborhood": "横田", "banchi": "516番地", "postal_code": "2891297", "old_code": "28912", "post_office": "日向", "type": "office", "multiple": false, "new": true, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "ヨコタ", "alternates": []}');
 INSERT INTO office_data VALUES('2891298','{"jis": "12237", "kana": "サンムシ サンブノモリコウリユウセンタ- アララギカン", "name": "山武市　さんぶの森交流センター　あららぎ館", "prefecture": "千葉県", "city": "山武市", "neighborhood": "埴谷", "banchi": "1884-1", "postal_code": "2891298", "old_code": "28912", "post_office": "日向", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "ハニヤ", "alternates": []}');
 INSERT INTO office_data VALUES('2891392','{"jis": "12237", "kana": "サンムシヤクシヨ", "name": "山武市役所", "prefecture": "千葉県", "city": "山武市", "neighborhood": "殿台", "banchi": "296", "postal_code": "2891392", "old_code": "28913", "post_office": "成東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "トノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2891593','{"jis": "12237", "kana": "サンムシ マツオアイテイ-ホケンフクシセンタ-", "name": "山武市　松尾ＩＴ保健福祉センター", "prefecture": "千葉県", "city": "山武市", "neighborhood": "松尾町五反田", "banchi": "3012", "postal_code": "2891593", "old_code": "28915", "post_office": "松尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "マツオマチゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('2891594','{"jis": "12237", "kana": "チバケンリツ マツオコウトウガツコウ", "name": "千葉県立　松尾高等学校", "prefecture": "千葉県", "city": "山武市", "neighborhood": "松尾町大堤", "banchi": "546", "postal_code": "2891594", "old_code": "28915", "post_office": "松尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "マツオマチオオツツミ", "alternates": []}');
 INSERT INTO office_data VALUES('2891592','{"jis": "12237", "kana": "ピ-デイ-ア-ルフア-マ カブシキガイシヤ チバコウジヨウ", "name": "ＰＤＲファーマ　株式会社　千葉工場", "prefecture": "千葉県", "city": "山武市", "neighborhood": "松尾町下大蔵", "banchi": "453番地1", "postal_code": "2891592", "old_code": "28915", "post_office": "松尾", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "マツオマチシモオオクラ", "alternates": []}');
 INSERT INTO office_data VALUES('2891892','{"jis": "12237", "kana": "サンムシ ハスヌマシユツチヨウジヨ", "name": "山武市　蓮沼出張所", "prefecture": "千葉県", "city": "山武市", "neighborhood": "蓮沼ハ", "banchi": "233番地", "postal_code": "2891892", "old_code": "28918", "post_office": "蓮沼", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "サンムシ", "neighborhood_kana": "ハスヌマハ", "alternates": []}');
 INSERT INTO office_data VALUES('2988501','{"jis": "12238", "kana": "イスミシヤクシヨ", "name": "いすみ市役所", "prefecture": "千葉県", "city": "いすみ市", "neighborhood": "大原", "banchi": "7400-1", "postal_code": "2988501", "old_code": "298  ", "post_office": "大原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "チバケン", "city_kana": "イスミシ", "neighborhood_kana": "オオハラ", "alternates": []}');
@@ -125520,15 +125571,14 @@
 INSERT INTO office_data VALUES('1018355','{"jis": "13101", "kana": "カブシキガイシヤ アサヒシユツパンシヤ", "name": "株式会社　朝日出版社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目3-5", "postal_code": "1018355", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018558','{"jis": "13101", "kana": "カブシキガイシヤ イワキ", "name": "株式会社　イワキ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "2丁目6-6", "postal_code": "1018558", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018201','{"jis": "13101", "kana": "カブシキガイシヤ インテ-ジ", "name": "株式会社　インテージ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田練塀町", "banchi": "3番地インテージ秋葉原ビル", "postal_code": "1018201", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダネリベイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018204','{"jis": "13101", "kana": "カブシキガイシヤ インテ-ジ・アソシエイツ", "name": "株式会社　インテージ・アソシエイツ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田練塀町", "banchi": "3インテージ秋葉原ビル", "postal_code": "1018204", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダネリベイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018460','{"jis": "13101", "kana": "カブシキガイシヤ オ-ムシヤ", "name": "株式会社　オーム社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目1", "postal_code": "1018460", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018461','{"jis": "13101", "kana": "カブシキガイシヤ オオゾラシユツパン", "name": "株式会社　宙出版", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目17番地廣瀬第1ビル", "postal_code": "1018461", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018624','{"jis": "13101", "kana": "カブシキガイシヤ カンソウシン", "name": "株式会社　かんそうしん", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目18-10", "postal_code": "1018624", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018476','{"jis": "13101", "kana": "カブシキガイシヤ キツズステ-シヨン", "name": "（株）　キッズステーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目26一ツ橋SIビル10階", "postal_code": "1018476", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018589','{"jis": "13101", "kana": "カブシキガイシヤ キヨクトウシヨウカイ/カブシキガイシヤ カパス", "name": "株式会社　極東商会／株式会社　カパス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-10-6", "postal_code": "1018589", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018672','{"jis": "13101", "kana": "カブシキガイシヤ キヨクトウシヨテン", "name": "株式会社　極東書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2-7-10帝都三崎町ビル(神田郵便局私書箱第72号)", "postal_code": "1018672", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018568','{"jis": "13101", "kana": "カブシキガイシヤ コクゴ", "name": "株式会社　コクゴ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "25", "postal_code": "1018568", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018410','{"jis": "13101", "kana": "カブシキガイシヤ シノテスト", "name": "株式会社　シノテスト", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3-7-9", "postal_code": "1018410", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018448','{"jis": "13101", "kana": "カブシキガイシヤ シマヅセイサクシヨ トウキヨウシシヤ", "name": "株式会社　島津製作所　東京支社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目3", "postal_code": "1018448", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018522','{"jis": "13101", "kana": "カブシキガイシヤ シヤカイホケンケンキユウシヨ", "name": "株式会社　社会保険研究所", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2-15-9TheKanda282", "postal_code": "1018522", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018050','{"jis": "13101", "kana": "カブシキガイシヤ シユウエイシヤ", "name": "株式会社　集英社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目5-10", "postal_code": "1018050", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
@@ -125550,37 +125600,35 @@
 INSERT INTO office_data VALUES('1018470','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムエス", "name": "株式会社　ディーエムエス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11", "postal_code": "1018470", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018667','{"jis": "13101", "kana": "カブシキガイシヤ デツク", "name": "株式会社　デック", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目23(神田郵便局私書箱第2号)", "postal_code": "1018667", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018631','{"jis": "13101", "kana": "カブシキガイシヤ トウワエンジニアリング", "name": "株式会社　東和エンジニアリング", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "1-7-8ユニゾ東神田一丁目ビル", "postal_code": "1018631", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018548','{"jis": "13101", "kana": "カブシキガイシヤ トクリキホンテン", "name": "株式会社　徳力本店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "鍛冶町", "banchi": "2丁目9番12号", "postal_code": "1018548", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018323','{"jis": "13101", "kana": "カブシキガイシヤ ニホンケイザイコウコクシヤ", "name": "株式会社　日本経済広告社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "2丁目10", "postal_code": "1018323", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018359','{"jis": "13101", "kana": "カブシキガイシヤ ニホンボウエキホケン", "name": "株式会社　日本貿易保険", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目8-1千代田ファーストビル", "postal_code": "1018359", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018561','{"jis": "13101", "kana": "カブシキガイシヤ ニホンマンパワ-", "name": "株式会社　日本マンパワー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田東松下町", "banchi": "47-1", "postal_code": "1018561", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダヒガシマツシタチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018901','{"jis": "13101", "kana": "カブシキガイシヤ ニホンマンパワ-ナイ カンポエルシ-ジムキヨク", "name": "株式会社　日本マンパワー内かんぽＬＣ事務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田東松下町", "banchi": "47-1", "postal_code": "1018901", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダヒガシマツシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018565','{"jis": "13101", "kana": "カブシキガイシヤ ヒガシニツポンギンコウ カンダシテン", "name": "株式会社　東日本銀行　神田支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "2", "postal_code": "1018565", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018562','{"jis": "13101", "kana": "カブシキガイシヤ ヒガシニツポンギンコウ ジムセンタ-", "name": "株式会社　東日本銀行　事務センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "2番地", "postal_code": "1018562", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018941','{"jis": "13101", "kana": "カブシキガイシヤ ヒタチビルシステム", "name": "株式会社　日立ビルシステム", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番", "postal_code": "1018941", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028644','{"jis": "13101", "kana": "カブシキガイシヤ ビ-エスニツポン(ビ-エスニツテレ)", "name": "株式会社　ビーエス日本（ビーエス日テレ）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "二番町", "banchi": "14番地日テレ麹町ビル南館3F", "postal_code": "1028644", "old_code": "101  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018189','{"jis": "13101", "kana": "カブシキガイシヤ フジヤクヒン", "name": "株式会社　富士薬品", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目2番地1KANDASQUARE9階", "postal_code": "1018189", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018405','{"jis": "13101", "kana": "カブシキガイシヤ フタミシヨボウ", "name": "株式会社　二見書房", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目18-11堀内三崎町ビル", "postal_code": "1018405", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018423','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンエ-ジエンシ-", "name": "株式会社　放送出版エージェンシー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-7-3神保町NKビル", "postal_code": "1018423", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018424','{"jis": "13101", "kana": "カブシキガイシヤ ホウソウシユツパンプロモ-シヨン ニホンアマチユアカヨウレンメイ ホンブジムキヨク", "name": "株式会社　放送出版プロモーション　日本アマチュア歌謡連盟　本部事務局", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-7-3神保町NKビル", "postal_code": "1018424", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018972','{"jis": "13101", "kana": "カブシキガイシヤ ミツウロコ", "name": "株式会社　ミツウロコ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1", "postal_code": "1018972", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018648','{"jis": "13101", "kana": "カブシキガイシヤ ヤクジニツポウシヤ", "name": "株式会社　薬事日報社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018648", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018524','{"jis": "13101", "kana": "カブシキガイシヤ ユニ・プランニング", "name": "株式会社　ユニ・プランニング", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "1丁目12-12美土代ビル4F", "postal_code": "1018524", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018325','{"jis": "13101", "kana": "カンコウギヨウケンコウホケンクミアイ", "name": "管工業健康保険組合", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目1", "postal_code": "1018325", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018464','{"jis": "13101", "kana": "カンダゼイムシヨ", "name": "神田税務署", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目3", "postal_code": "1018464", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018712','{"jis": "13101", "kana": "カンダブツサン", "name": "神田物産　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-13(神田郵便局私書箱第122号)", "postal_code": "1018712", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018351','{"jis": "13101", "kana": "ガツコウホウジン オオハラガクエン", "name": "学校法人　大原学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "2丁目4-11大原簿記学校本館", "postal_code": "1018351", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018433','{"jis": "13101", "kana": "ガツコウホウジン キヨウリツジヨシガクエン", "name": "学校法人　共立女子学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目2-1", "postal_code": "1018433", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018313','{"jis": "13101", "kana": "ガツコウホウジン スルガダイガクエン スンダイヨビガツコウ", "name": "学校法人　駿河台学園　駿台予備学校", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-17", "postal_code": "1018313", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018456','{"jis": "13101", "kana": "ガツコウホウジン セイソクガクエン", "name": "学校法人　正則学園", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目1", "postal_code": "1018456", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018301','{"jis": "13101", "kana": "ガツコウホウジン メイジダイガク", "name": "学校法人　明治大学", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目1", "postal_code": "1018301", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018437','{"jis": "13101", "kana": "キヨウリツジヨシダイガク", "name": "共立女子大学", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目2-1", "postal_code": "1018437", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018621','{"jis": "13101", "kana": "キヨウリツメンテナンス", "name": "（株）　共立メンテナンス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "2丁目18-8", "postal_code": "1018621", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
-INSERT INTO office_data VALUES('1018311','{"jis": "13101", "kana": "キヨウリンセイヤク カブシキガイシヤ", "name": "杏林製薬　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018311", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
+INSERT INTO office_data VALUES('1018311','{"jis": "13101", "kana": "キヨウリンセイヤク カブシキガイシヤ", "name": "杏林製薬　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6", "postal_code": "1018311", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018645','{"jis": "13101", "kana": "キリンビバレツジ カブシキガイシヤ", "name": "キリンビバレッジ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018645", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018977','{"jis": "13101", "kana": "グロ-リ- カブシキカイシヤ トウキヨウホンブ", "name": "グローリー　株式会社　東京本部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDXビル19F", "postal_code": "1018977", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018372','{"jis": "13101", "kana": "コウエキザイダンホウジン ケツカクヨボウカイ ソウゴウケンシンスイシンセンタ-", "name": "公益財団法人　結核予防会　総合健診推進センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "1丁目3-12", "postal_code": "1018372", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018378','{"jis": "13101", "kana": "コウエキシヤダンホウジン ゼンニホンビヨウインキヨウカイ", "name": "公益社団法人　全日本病院協会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "猿楽町", "banchi": "2丁目8番8号住友不動産猿楽町ビル7階", "postal_code": "1018378", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018307','{"jis": "13101", "kana": "コウエキシヤダンホウジン ニホンカガクカイ", "name": "公益社団法人　日本化学会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目5", "postal_code": "1018307", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018559','{"jis": "13101", "kana": "サトウキンゾク カブシキガイシヤ", "name": "佐藤金属　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "2丁目13", "postal_code": "1018559", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018682','{"jis": "13101", "kana": "サンヨウボウエキ", "name": "三洋貿易　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目11(神田郵便局私書箱第215号)", "postal_code": "1018682", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
@@ -125622,47 +125670,44 @@
 INSERT INTO office_data VALUES('1018688','{"jis": "13101", "kana": "ニチイガツカン", "name": "（株）　ニチイ学館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目9(神田郵便局私書箱第25号)", "postal_code": "1018688", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018329','{"jis": "13101", "kana": "ニツシンカサイカイジヨウホケン カブシキカイシヤ", "name": "日新火災海上保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目3番地", "postal_code": "1018329", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018441','{"jis": "13101", "kana": "ニツシンセイフン カブシキガイシヤ", "name": "日清製粉　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目25", "postal_code": "1018441", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018210','{"jis": "13101", "kana": "ニツポンカミツウシヨウ カブシキガイシヤ", "name": "日本紙通商　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目6番", "postal_code": "1018210", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018215','{"jis": "13101", "kana": "ニツポンセイシクレシア カブシキガイシヤ", "name": "日本製紙クレシア　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6", "postal_code": "1018215", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018213','{"jis": "13101", "kana": "ニツポンセイシモクザイ カブシキガイシヤ", "name": "日本製紙木材　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目6番", "postal_code": "1018213", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018647','{"jis": "13101", "kana": "ニツポンツウウン カブシキガイシヤ", "name": "日本通運　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "2番地", "postal_code": "1018647", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018946','{"jis": "13101", "kana": "ニツポンレンタカ-ア-バンネツト カブシキガイシヤ トウキヨウデイビジヨン", "name": "ニッポンレンタカーアーバンネット　株式会社　東京ディビジョン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "東神田", "banchi": "2丁目1-11第一坂本ビル", "postal_code": "1018946", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒガシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018710','{"jis": "13101", "kana": "ニホンシユツパンハンバイ", "name": "日本出版販売　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4丁目3(神田郵便局私書箱第13号)", "postal_code": "1018710", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018310','{"jis": "13101", "kana": "ニホンダイガク シガクブ", "name": "日本大学　歯学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目8-13", "postal_code": "1018310", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018354','{"jis": "13101", "kana": "ニホンダイガク ツウシンキヨウイクブ", "name": "日本大学　通信教育部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目2-3", "postal_code": "1018354", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018375','{"jis": "13101", "kana": "ニホンダイガク ホウガクブ", "name": "日本大学　法学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三崎町", "banchi": "2丁目3-1", "postal_code": "1018375", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('1018308','{"jis": "13101", "kana": "ニホンダイガク リコウガクブ", "name": "日本大学　理工学部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "1丁目8-14", "postal_code": "1018308", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018707','{"jis": "13101", "kana": "ニホンパ-ソナルセンタ-", "name": "（株）　日本パーソナルセンター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目5新須田町ビル3F(神田郵便局私書箱第209号)", "postal_code": "1018707", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018711','{"jis": "13101", "kana": "ハクセンシヤ", "name": "（株）　白泉社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "西神田", "banchi": "3丁目6-4(神田郵便局私書箱第92号)", "postal_code": "1018711", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ニシカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018605','{"jis": "13101", "kana": "ハシモトサンギヨウ", "name": "橋本産業　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田紺屋町", "banchi": "34", "postal_code": "1018605", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダコンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018462','{"jis": "13101", "kana": "パシフイツクコンサルタンツ カブシキガイシヤ", "name": "パシフィックコンサルタンツ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目22番地", "postal_code": "1018462", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018971','{"jis": "13101", "kana": "ヒタチデンセン カブシキガイシヤ", "name": "日立電線　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDX", "postal_code": "1018971", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018439','{"jis": "13101", "kana": "ヒトツバシダイガク チヨダキヤンパスジムシツ", "name": "一橋大学　千代田キャンパス事務室", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目1-2", "postal_code": "1018439", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018528','{"jis": "13101", "kana": "ピツプ カブシキガイシヤ", "name": "ピップ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3-3-7", "postal_code": "1018528", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018542','{"jis": "13101", "kana": "フジパン カブシキガイシヤ カントウジギヨウブ", "name": "フジパン　（株）　関東事業部", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田富山町", "banchi": "10-1", "postal_code": "1018542", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダトミヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018606','{"jis": "13101", "kana": "フマキラ- カブシキガイシヤ", "name": "フマキラー　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美倉町", "banchi": "11", "postal_code": "1018606", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミクラチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018970','{"jis": "13101", "kana": "フルカワスカイ カブシキガイシヤ", "name": "古河スカイ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4丁目14-1秋葉原UDX", "postal_code": "1018970", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018477','{"jis": "13101", "kana": "ミズノ カブシキガイシヤ", "name": "ミズノ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "3丁目22", "postal_code": "1018477", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018219','{"jis": "13101", "kana": "ミズホシヨウケン カブシキガイシヤ", "name": "みずほ証券　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "4-6御茶ノ水ソラシティ", "postal_code": "1018219", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
+INSERT INTO office_data VALUES('1018443','{"jis": "13101", "kana": "ミズホリサ-チアンドテクノロジ-ズ カブシキガイシヤ", "name": "みずほリサーチ＆テクノロジーズ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "2丁目3", "postal_code": "1018443", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018429','{"jis": "13101", "kana": "ミタニサンギヨウ カブシキガイシヤ", "name": "三谷産業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2-36-1千代田ファーストウイング", "postal_code": "1018429", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018485','{"jis": "13101", "kana": "ミツイカガクトウセロ カブシキガイシヤ", "name": "三井化学東セロ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7", "postal_code": "1018485", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018011','{"jis": "13101", "kana": "ミツイスミトモカイジヨウカサイホケン カブシキカイシヤ", "name": "三井住友海上火災保険　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "3丁目9(神田郵便局私書箱第23号)", "postal_code": "1018011", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018338','{"jis": "13101", "kana": "ミツビシマテリアル カブシキガイシヤ", "name": "三菱マテリアル　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目16-11内神田渋谷ビル9階", "postal_code": "1018338", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018637','{"jis": "13101", "kana": "ミツビシユ-エフジエ-フアクタ- カブシキガイシヤ", "name": "三菱ＵＦＪファクター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番ワテラスタワー", "postal_code": "1018637", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018676','{"jis": "13101", "kana": "ムサシノギンコウ トウキヨウシテン", "name": "（株）　武蔵野銀行　東京支店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "2丁目15-9(神田郵便局私書箱第45号)", "postal_code": "1018676", "old_code": "101  ", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018554','{"jis": "13101", "kana": "メタウオ-タ- カブシキガイシヤ", "name": "メタウォーター　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田須田町", "banchi": "1丁目25番", "postal_code": "1018554", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018626','{"jis": "13101", "kana": "ヤマキ カブシキガイシヤ", "name": "ヤマキ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "外神田", "banchi": "4-8-2", "postal_code": "1018626", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ソトカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018585','{"jis": "13101", "kana": "ヤマザキセイパン カブシキガイシヤ", "name": "山崎製パン　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "岩本町", "banchi": "3丁目10-1", "postal_code": "1018585", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イワモトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018580','{"jis": "13101", "kana": "ユアサシヨウジ カブシキガイシヤ", "name": "ユアサ商事　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田美土代町", "banchi": "7番住友不動産神田ビル", "postal_code": "1018580", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダミトシロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018531','{"jis": "13101", "kana": "ユウゲンガイシヤ カガクヒヨウロンシヤ", "name": "有限会社　科学評論社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田司町", "banchi": "2丁目10-15", "postal_code": "1018531", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダツカサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018422','{"jis": "13101", "kana": "ユウセントラベル", "name": "郵船トラベル　（株）", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "2丁目2", "postal_code": "1018422", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018336','{"jis": "13101", "kana": "リケンテクノス カブシキガイシヤ", "name": "リケンテクノス　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田淡路町", "banchi": "2丁目101番地ワテラスタワー", "postal_code": "1018336", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダアワジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018446','{"jis": "13101", "kana": "リヨウエイ カブシキカイシヤ", "name": "菱栄　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "1丁目13大手町宝栄ビル7階", "postal_code": "1018446", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1018315','{"jis": "13101", "kana": "ロウドウキンコカイカン", "name": "労働金庫会館", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目5-15", "postal_code": "1018315", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018642','{"jis": "13101", "kana": "ワイケイケイ カブシキガイシヤ", "name": "ＹＫＫ　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田和泉町", "banchi": "1", "postal_code": "1018642", "old_code": "101  ", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダイズミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1018002','{"jis": "13101", "kana": "カブシキガイシヤ イワナミシヨテン", "name": "株式会社　岩波書店", "prefecture": "東京都", "city": "千代田区", "neighborhood": "一ツ橋", "banchi": "2丁目5-5", "postal_code": "1018002", "old_code": "10102", "post_office": "神田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ヒトツバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1018654','{"jis": "13101", "kana": "イシフクキンゾクコウギヨウ カブシキガイシヤ", "name": "石福金属興業　株式会社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "内神田", "banchi": "3丁目20-7(神田郵便局私書箱第57号)", "postal_code": "1018654", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "ウチカンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1018701','{"jis": "13101", "kana": "カブシキガイシヤ シヨウデンシヤ", "name": "株式会社　祥伝社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田神保町", "banchi": "3丁目6-5(神田郵便局私書箱第152号)", "postal_code": "1018701", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダジンボウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1048650','{"jis": "13101", "kana": "カブシキガイシヤ デイ-エムエス", "name": "株式会社　ディーエムエス", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田小川町", "banchi": "1丁目11(晴海郵便局私書箱第230号)", "postal_code": "1048650", "old_code": "10191", "post_office": "晴海", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダオガワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1018718','{"jis": "13101", "kana": "カブシキガイシヤ ニホンイジシンポウシヤ", "name": "株式会社　日本醫事新報社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田駿河台", "banchi": "2丁目9(神田郵便局私書箱第18号)", "postal_code": "1018718", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダスルガダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1018715','{"jis": "13101", "kana": "ゼンニホンシヨゲイブンカイン", "name": "全日本書芸文化院", "prefecture": "東京都", "city": "千代田区", "neighborhood": "神田錦町", "banchi": "3丁目20(神田郵便局私書箱第37号)", "postal_code": "1018715", "old_code": "10191", "post_office": "神田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "カンダニシキチョウ", "alternates": []}');
@@ -125719,15 +125764,15 @@
 INSERT INTO office_data VALUES('1028671','{"jis": "13101", "kana": "カブシキガイシヤ エルヴイジヨン", "name": "株式会社　エルヴィジョン", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段南", "banchi": "3丁目5-9(麹町郵便局私書箱第98号)", "postal_code": "1028671", "old_code": "102  ", "post_office": "麹町", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンミナミ", "alternates": []}');
 INSERT INTO office_data VALUES('1028349','{"jis": "13101", "kana": "カブシキガイシヤ オ-クネツト", "name": "株式会社　オークネット", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "8-1三番町東急ビル7F", "postal_code": "1028349", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028565','{"jis": "13101", "kana": "カブシキガイシヤ オ-タニコ-ポレ-シヨン", "name": "株式会社　オータニコーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "4-1", "postal_code": "1028565", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028573','{"jis": "13101", "kana": "カブシキガイシヤ オオツカシヨウカイ", "name": "株式会社　大塚商会", "prefecture": "東京都", "city": "千代田区", "neighborhood": "飯田橋", "banchi": "2丁目18-4", "postal_code": "1028573", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "イイダバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1028025','{"jis": "13101", "kana": "カブシキガイシヤ オズマピ-ア-ル", "name": "株式会社　オズマピーアール", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-23", "postal_code": "1028025", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028503','{"jis": "13101", "kana": "カブシキガイシヤ オリエントコ-ポレ-シヨン", "name": "株式会社　オリエントコーポレーション", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "5丁目2-1", "postal_code": "1028503", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028504','{"jis": "13101", "kana": "カブシキガイシヤ オリエントコ-ポレ-シヨン シユトケンカンリセンタ-", "name": "株式会社　オリエントコーポレーション　首都圏管理センター", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "5丁目2-1", "postal_code": "1028504", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1028301','{"jis": "13101", "kana": "カブシキガイシヤ カ-・アンド・ドライバ-", "name": "株式会社　カー・アンド・ドライバー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目6番9号DIK麹町ビル703号室", "postal_code": "1028301", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
+INSERT INTO office_data VALUES('1028301','{"jis": "13101", "kana": "カブシキガイシヤ カ-・アンド・ドライバ-", "name": "株式会社　カー・アンド・ドライバー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "1丁目6番9号DIK麹町ビル703号室", "postal_code": "1028301", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028622','{"jis": "13101", "kana": "カブシキガイシヤ カ-ビユ-", "name": "株式会社　カービュー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "1番3号東京ガーデンテラス紀尾井町紀尾井タワー22階", "postal_code": "1028622", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028191','{"jis": "13101", "kana": "カブシキガイシヤ カテイガホウビジネスパ-トナ-ズ", "name": "株式会社　家庭画報ビジネスパートナーズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "4-2-29", "postal_code": "1028191", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028685','{"jis": "13101", "kana": "カブシキガイシヤ カドカワヘラルド・ピクチヤ-ズ", "name": "株式会社　角川ヘラルド・ピクチャーズ", "prefecture": "東京都", "city": "千代田区", "neighborhood": "紀尾井町", "banchi": "3-6紀尾井町パークビル8F", "postal_code": "1028685", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "キオイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028540','{"jis": "13101", "kana": "カブシキガイシヤ カンキシユツパン", "name": "株式会社　かんき出版", "prefecture": "東京都", "city": "千代田区", "neighborhood": "麹町", "banchi": "4丁目1-4西脇ビル", "postal_code": "1028540", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "コウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1028228','{"jis": "13101", "kana": "カブシキガイシヤ カント-", "name": "株式会社　カントー", "prefecture": "東京都", "city": "千代田区", "neighborhood": "九段北", "banchi": "1丁目11-2", "postal_code": "1028228", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "クダンキタ", "alternates": []}');
 INSERT INTO office_data VALUES('1028522','{"jis": "13101", "kana": "カブシキガイシヤ キヨウドウセンデン", "name": "株式会社　協同宣伝", "prefecture": "東京都", "city": "千代田区", "neighborhood": "三番町", "banchi": "3-8泉館三番町", "postal_code": "1028522", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "サンバンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1028152','{"jis": "13101", "kana": "カブシキガイシヤ ケンキユウシヤホンシヤ", "name": "株式会社　研究社本社", "prefecture": "東京都", "city": "千代田区", "neighborhood": "富士見", "banchi": "2丁目11-3", "postal_code": "1028152", "old_code": "102  ", "post_office": "麹町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チヨダク", "neighborhood_kana": "フジミ", "alternates": []}');
@@ -126071,15 +126116,14 @@
 INSERT INTO office_data VALUES('1038234','{"jis": "13102", "kana": "ダイイチサンキヨウ カブシキガイシヤ ダイイチサンキヨウニホンバシビル", "name": "第一三共　株式会社　第一三共日本橋ビル", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "3-14-10", "postal_code": "1038234", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038425','{"jis": "13102", "kana": "ダイケンコウギヨウ (カブ)", "name": "大建工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "2丁目7-1", "postal_code": "1038425", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038511','{"jis": "13102", "kana": "ダイトウボウ カブシキガイシヤ", "name": "ダイトウボウ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "1-6-1丸柏タマビル7階", "postal_code": "1038511", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038383','{"jis": "13102", "kana": "ダイニチセイカコウギヨウ (カブ)", "name": "大日精化工業　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋馬喰町", "banchi": "1丁目7-6", "postal_code": "1038383", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシバクロチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038240','{"jis": "13102", "kana": "ダイワセイカン (カブ)", "name": "大和製罐　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "2丁目1-10", "postal_code": "1038240", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038324','{"jis": "13102", "kana": "チユウガイセイヤク カブシキガイシヤ", "name": "中外製薬　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "2丁目1-1日本橋三井タワー15F", "postal_code": "1038324", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038404','{"jis": "13102", "kana": "ツカモト (カブ)", "name": "ツカモト　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋本町", "banchi": "1丁目6-5", "postal_code": "1038404", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホンチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('1038423','{"jis": "13102", "kana": "デイ-エムミツイセイトウ カブシキガイシヤ", "name": "ＤＭ三井製糖　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋箱崎町", "banchi": "36-2Daiwaリバーゲート12階", "postal_code": "1038423", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシハコザキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038233','{"jis": "13102", "kana": "デイアイシ- カブシキガイシヤ", "name": "ＤＩＣ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋", "banchi": "3丁目7-20", "postal_code": "1038233", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038338','{"jis": "13102", "kana": "デンカ カブシキカイシヤ", "name": "デンカ　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋室町", "banchi": "二丁目1番1号", "postal_code": "1038338", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシムロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1038566','{"jis": "13102", "kana": "デンヨ- カブシキガイシヤ", "name": "デンヨー　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "2丁目8-5", "postal_code": "1038566", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038554','{"jis": "13102", "kana": "トウキヨウオリモノケンコウホケンクミアイ", "name": "東京織物健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋堀留町", "banchi": "1丁目9-6", "postal_code": "1038554", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシホリドメチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1038465','{"jis": "13102", "kana": "トウキヨウジツギヨウケンコウホケンクミアイ", "name": "東京実業健康保険組合", "prefecture": "東京都", "city": "中央区", "neighborhood": "東日本橋", "banchi": "3丁目10-4", "postal_code": "1038465", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヒガシニホンバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1038285','{"jis": "13102", "kana": "トウキヨウタテモノ カブシキガイシヤ", "name": "東京建物　株式会社", "prefecture": "東京都", "city": "中央区", "neighborhood": "八重洲", "banchi": "1丁目4番16号", "postal_code": "1038285", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ヤエス", "alternates": []}');
 INSERT INTO office_data VALUES('1038360','{"jis": "13102", "kana": "トウキヨウトニホンバシトクベツシユツチヨウジヨ", "name": "東京都中央区日本橋特別出張所", "prefecture": "東京都", "city": "中央区", "neighborhood": "日本橋蛎殻町", "banchi": "1丁目31-1", "postal_code": "1038360", "old_code": "103  ", "post_office": "日本橋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ニホンバシカキガラチョウ", "alternates": []}');
@@ -126221,16 +126265,14 @@
 INSERT INTO office_data VALUES('1048380','{"jis": "13102", "kana": "カブシキガイシヤ ニツポコ-ポレ-シヨン", "name": "株式会社　ＮＩＰＰＯコーポレーション", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "1丁目19-11", "postal_code": "1048380", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048176','{"jis": "13102", "kana": "カブシキガイシヤ ニホンケイザイシヤ", "name": "株式会社　日本経済社", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "7丁目13-20", "postal_code": "1048176", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048208','{"jis": "13102", "kana": "カブシキガイシヤ ノエビア", "name": "株式会社　ノエビア", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "7丁目6-15", "postal_code": "1048208", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048132','{"jis": "13102", "kana": "カブシキガイシヤ ハクヒンカン", "name": "株式会社　博品館", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "8丁目8-11", "postal_code": "1048132", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048304','{"jis": "13102", "kana": "カブシキガイシヤ パイロツトコ-ポレ-シヨン", "name": "株式会社　パイロットコーポレーション", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "2丁目6番21号", "postal_code": "1048304", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1048240','{"jis": "13102", "kana": "カブシキガイシヤ ヒサヤダイコクドウ", "name": "株式会社　ヒサヤ大黒堂", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "1丁目6-1クレッセントビル3F", "postal_code": "1048240", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048505','{"jis": "13102", "kana": "カブシキガイシヤ ヒノデシユツパン", "name": "株式会社　日之出出版", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "5-6-10浜離宮パークサイドプレイス7階", "postal_code": "1048505", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
-INSERT INTO office_data VALUES('1048572','{"jis": "13102", "kana": "カブシキガイシヤ ピ-エスミツビシ トウキヨウドボク・ケンチクシテン", "name": "株式会社　ピーエス三菱　東京土木・建築支店", "prefecture": "東京都", "city": "中央区", "neighborhood": "晴海", "banchi": "2丁目5-24晴海センタービル2階", "postal_code": "1048572", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハルミ", "alternates": []}');
-INSERT INTO office_data VALUES('1048215','{"jis": "13102", "kana": "カブシキガイシヤ ピ-エスミツビシ ホンシヤ", "name": "株式会社　ピーエス三菱　本社", "prefecture": "東京都", "city": "中央区", "neighborhood": "晴海", "banchi": "2丁目5-24晴海センタービル3階", "postal_code": "1048215", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ハルミ", "alternates": []}');
 INSERT INTO office_data VALUES('1048340','{"jis": "13102", "kana": "カブシキガイシヤ ブリヂストン", "name": "株式会社　ブリヂストン", "prefecture": "東京都", "city": "中央区", "neighborhood": "京橋", "banchi": "3-1-1", "postal_code": "1048340", "old_code": "104  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "キョウバシ", "alternates": []}');
 INSERT INTO office_data VALUES('1008621','{"jis": "13102", "kana": "カブシキガイシヤ プランニングオフイス トライ・アングル", "name": "株式会社　プランニングオフィス　トライ・アングル", "prefecture": "東京都", "city": "中央区", "neighborhood": "築地", "banchi": "1丁目5-4(銀座郵便局私書箱第366号)", "postal_code": "1008621", "old_code": "104  ", "post_office": "銀座", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ツキジ", "alternates": []}');
 INSERT INTO office_data VALUES('1048104','{"jis": "13102", "kana": "カブシキガイシヤ ホウケン", "name": "株式会社　法研", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "1丁目10-1", "postal_code": "1048104", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048003','{"jis": "13102", "kana": "カブシキガイシヤ マガジンハウス", "name": "株式会社　マガジンハウス", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目13-10", "postal_code": "1048003", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048130','{"jis": "13102", "kana": "カブシキガイシヤ マツヤ ギンザホンテン", "name": "株式会社　松屋　銀座本店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "3丁目6-1", "postal_code": "1048130", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048145','{"jis": "13102", "kana": "カブシキガイシヤ ミキモト ギンザヨンチヨウメホンテン", "name": "株式会社　ミキモト　銀座４丁目本店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "4-5-5", "postal_code": "1048145", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
 INSERT INTO office_data VALUES('1048212','{"jis": "13102", "kana": "カブシキガイシヤ ミツコシ ギンザテン", "name": "株式会社　三越　銀座店", "prefecture": "東京都", "city": "中央区", "neighborhood": "銀座", "banchi": "4丁目6-16", "postal_code": "1048212", "old_code": "104  ", "post_office": "銀座", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "チュウオウク", "neighborhood_kana": "ギンザ", "alternates": []}');
@@ -126755,15 +126797,15 @@
 INSERT INTO office_data VALUES('1088212','{"jis": "13103", "kana": "エフ・デイ-・ケイ カブシキカイシヤ", "name": "ＦＤＫ　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-6-41品川クリスタルスクエア8F", "postal_code": "1088212", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088361','{"jis": "13103", "kana": "オ-ストラリアタイシカン オ-ストラリアエンバシイ", "name": "オーストラリア大使館　ＡＵＳＴＲＡＬＩＡＮ　ＥＭＢＡＳＳＹ", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "2丁目1-14", "postal_code": "1088361", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088242','{"jis": "13103", "kana": "オオツカセイヤク カブシキガイシヤ", "name": "大塚製薬　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16番4号品川グランドセントラルタワー", "postal_code": "1088242", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088241','{"jis": "13103", "kana": "オオツカホ-ルデイングス カブシキガイシヤ", "name": "大塚ホールディングス　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16-4品川グランドセントラルタワー", "postal_code": "1088241", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088551','{"jis": "13103", "kana": "オキデンキコウギヨウ カブシキガイシヤ", "name": "沖電気工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目10-16", "postal_code": "1088551", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088386','{"jis": "13103", "kana": "オツクスフオ-ドダイガクシユツパンキヨク カブシキガイシヤ", "name": "オックスフォード大学出版局　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "4-17-5田町プレイスビル3F", "postal_code": "1088386", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088379','{"jis": "13103", "kana": "カブシキカイシヤ インボイス", "name": "株式会社　インボイス", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "1-3-13", "postal_code": "1088379", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
-INSERT INTO office_data VALUES('1088505','{"jis": "13103", "kana": "カブシキカイシヤ エヌ・テイ・テイ・デ-タ", "name": "株式会社　ＮＴＴデータ", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-9-1", "postal_code": "1088505", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
+INSERT INTO office_data VALUES('1088505','{"jis": "13103", "kana": "カブシキカイシヤ エヌ・テイ・テイ・デ-タ", "name": "株式会社　ＮＴＴデータ", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-9-1", "postal_code": "1088505", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088220','{"jis": "13103", "kana": "カブシキカイシヤ タンセイシヤ", "name": "株式会社　丹青社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "1-2-70品川シーズンテラス19F・20F", "postal_code": "1088220", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088250','{"jis": "13103", "kana": "カブシキカイシヤ ヒタチセイサクシヨ ジヨウホウ・ツウシンシステムシヤ", "name": "株式会社　日立製作所　情報・通信システム社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目18-1JR品川イーストビル", "postal_code": "1088250", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088301','{"jis": "13103", "kana": "カブシキガイシヤ アイスタ-シヨウジ", "name": "株式会社　アイスター商事", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1-4-28三田国際ビル10F", "postal_code": "1088301", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088553','{"jis": "13103", "kana": "カブシキガイシヤ アイテイ-サ-ビス シバウラジギヨウシヨ", "name": "株式会社　ＩＴサービス　芝浦事業所", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目9-25芝浦スクエアビル15F", "postal_code": "1088553", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1088308','{"jis": "13103", "kana": "カブシキガイシヤ アサヒリヨコウ", "name": "株式会社　朝日旅行", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3-13-12三田MTビル2F", "postal_code": "1088308", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088313','{"jis": "13103", "kana": "カブシキガイシヤ イツテン", "name": "株式会社　一点", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1-4-28三田国際ビル10F", "postal_code": "1088313", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088305','{"jis": "13103", "kana": "カブシキガイシヤ エヌイ-シ-ライベツクス", "name": "株式会社　ＮＥＣライベックス", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4-28", "postal_code": "1088305", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
@@ -126908,15 +126950,15 @@
 INSERT INTO office_data VALUES('1088215','{"jis": "13103", "kana": "ミツビシジユウコウギヨウ カブシキガイシヤ", "name": "三菱重工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "港南", "banchi": "2丁目16番5号", "postal_code": "1088215", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "コウナン", "alternates": []}');
 INSERT INTO office_data VALUES('1088315','{"jis": "13103", "kana": "ミナトク ミナトホケンジヨ", "name": "港区　みなと保健所", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4番10号", "postal_code": "1088315", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088636','{"jis": "13103", "kana": "メイジガクインダイガク", "name": "明治学院大学", "prefecture": "東京都", "city": "港区", "neighborhood": "白金台", "banchi": "1丁目2-37", "postal_code": "1088636", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シロカネダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1088403','{"jis": "13103", "kana": "モリナガセイカ カブシキガイシヤ", "name": "森永製菓　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目33-1", "postal_code": "1088403", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088384','{"jis": "13103", "kana": "モリナガニユウギヨウ カブシキガイシヤ", "name": "森永乳業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目33-1", "postal_code": "1088384", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088333','{"jis": "13103", "kana": "ヤザキソウギヨウ カブシキガイシヤ", "name": "矢崎総業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "1丁目4-28", "postal_code": "1088333", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088568','{"jis": "13103", "kana": "ヤマハ カブシキガイシヤ トウキヨウエイギヨウジムシヨ", "name": "ヤマハ　株式会社　東京営業事務所", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "2丁目17-11", "postal_code": "1088568", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
-INSERT INTO office_data VALUES('1088575','{"jis": "13103", "kana": "ユニ・チヤ-ム カブシキガイシヤ", "name": "ユニ・チャーム　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3-5-19住友不動産東京三田ガーデンタワー", "postal_code": "1088575", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
+INSERT INTO office_data VALUES('1088575','{"jis": "13103", "kana": "ユニ・チヤ-ム カブシキガイシヤ", "name": "ユニ・チャーム　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3-5-19住友不動産東京三田ガーデンタワー", "postal_code": "1088575", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088388','{"jis": "13103", "kana": "ヨコハマカセイ カブシキガイシヤ", "name": "横浜化成　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "高輪", "banchi": "2-21-43YCC高輪ビル", "postal_code": "1088388", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "タカナワ", "alternates": []}');
 INSERT INTO office_data VALUES('1088385','{"jis": "13103", "kana": "リソウカガクコウギヨウ カブシキガイシヤ", "name": "理想科学工業　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5-34-7田町センタービル", "postal_code": "1088385", "old_code": "108  ", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1088001','{"jis": "13103", "kana": "ニツポンデンキ カブシキガイシヤ", "name": "日本電気　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "芝", "banchi": "5丁目7-1NEC本社ビル", "postal_code": "1088001", "old_code": "10801", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバ", "alternates": []}');
 INSERT INTO office_data VALUES('1086363','{"jis": "13103", "kana": "エスエムビ-シ-デンシサイケンキロク カブシキガイシヤ", "name": "ＳＭＢＣ電子債権記録　株式会社", "prefecture": "東京都", "city": "港区", "neighborhood": "三田", "banchi": "3丁目5番27号住友不動産三田ツインビル西館7階", "postal_code": "1086363", "old_code": "10863", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ミタ", "alternates": []}');
 INSERT INTO office_data VALUES('1088071','{"jis": "13103", "kana": "カブシキガイシヤ ジヤパンタイムズ", "name": "株式会社　ジャパンタイムズ", "prefecture": "東京都", "city": "港区", "neighborhood": "芝浦", "banchi": "4丁目5-4", "postal_code": "1088071", "old_code": "10871", "post_office": "高輪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "シバウラ", "alternates": []}');
 INSERT INTO office_data VALUES('1358707','{"jis": "13103", "kana": "アクアシテイオダイバ", "name": "アクアシティお台場", "prefecture": "東京都", "city": "港区", "neighborhood": "台場", "banchi": "1丁目7番1号", "postal_code": "1358707", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ダイバ", "alternates": []}');
 INSERT INTO office_data VALUES('1358625','{"jis": "13103", "kana": "カブシキガイシヤ トウキヨウヒユ-マニアエンタプライズ", "name": "株式会社　東京ヒューマニアエンタプライズ", "prefecture": "東京都", "city": "港区", "neighborhood": "台場", "banchi": "1丁目9-1", "postal_code": "1358625", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ミナトク", "neighborhood_kana": "ダイバ", "alternates": []}');
@@ -126984,15 +127026,14 @@
 INSERT INTO office_data VALUES('1608334','{"jis": "13104", "kana": "カブシキガイシヤ ミマツ", "name": "株式会社　三松", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目2-11新宿三井2号館14F", "postal_code": "1608334", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608486','{"jis": "13104", "kana": "カブシキガイシヤ ヨドバシカメラ", "name": "株式会社　ヨドバシカメラ", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "5-3-1", "postal_code": "1608486", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638680','{"jis": "13104", "kana": "カブシキガイシヤ ロツテリア", "name": "（株）　ロッテリア", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "3丁目20-1(新宿郵便局私書箱第310号)", "postal_code": "1638680", "old_code": "160  ", "post_office": "新宿", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608580','{"jis": "13104", "kana": "カブシキガイシヤ ワニマガジンシヤ", "name": "株式会社　ワニマガジン社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "内藤町", "banchi": "1", "postal_code": "1608580", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ナイトウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1608403','{"jis": "13104", "kana": "カワベ カブシキガイシヤ", "name": "川辺　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷", "banchi": "4丁目16-3日本生命新宿御苑前ビル", "postal_code": "1608403", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤ", "alternates": []}');
 INSERT INTO office_data VALUES('1608402','{"jis": "13104", "kana": "ガツコウホウジン トウキヨウイカダイガク", "name": "学校法人　東京医科大学", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "6丁目1-1", "postal_code": "1608402", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608422','{"jis": "13104", "kana": "キ-ウエアソリユ-シヨンズ カブシキガイシヤ", "name": "キーウェアソリューションズ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目1番13号", "postal_code": "1608422", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
-INSERT INTO office_data VALUES('1608308','{"jis": "13104", "kana": "クラブツ-リズム カブシキガイシヤ", "name": "クラブツーリズム　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目3-1新宿アイランドウイング", "postal_code": "1608308", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608582','{"jis": "13104", "kana": "ケイオウギジユクダイガク イガクブ", "name": "慶應義塾大学　医学部", "prefecture": "東京都", "city": "新宿区", "neighborhood": "信濃町", "banchi": "35", "postal_code": "1608582", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シナノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1638003','{"jis": "13104", "kana": "ケイデイデイアイ カブシキガイシヤ", "name": "ＫＤＤＩ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目3-2", "postal_code": "1638003", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1638535','{"jis": "13104", "kana": "ケイデイデイアイソウゴウサ-ビス カブシキガイシヤ", "name": "ＫＤＤＩ総合サービス　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "2丁目3-3KDDIビルアネックス", "postal_code": "1638535", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608374','{"jis": "13104", "kana": "ゲイノウカデンシヤ", "name": "芸能花伝舎", "prefecture": "東京都", "city": "新宿区", "neighborhood": "西新宿", "banchi": "6丁目12-30", "postal_code": "1608374", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ニシシンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608441','{"jis": "13104", "kana": "コウコクシヤ カブシキガイシヤ", "name": "廣告社　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "新宿", "banchi": "3丁目1番24号京王新宿三丁目ビル", "postal_code": "1608441", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "シンジュク", "alternates": []}');
 INSERT INTO office_data VALUES('1608521','{"jis": "13104", "kana": "コウメイキカンシキヨク", "name": "公明機関紙局", "prefecture": "東京都", "city": "新宿区", "neighborhood": "南元町", "banchi": "18", "postal_code": "1608521", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ミナミモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1608543','{"jis": "13104", "kana": "コモンズ カブシキガイシヤ", "name": "コモンズ　株式会社", "prefecture": "東京都", "city": "新宿区", "neighborhood": "四谷坂町", "banchi": "12番21号", "postal_code": "1608543", "old_code": "160  ", "post_office": "新宿", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シンジュクク", "neighborhood_kana": "ヨツヤサカマチ", "alternates": []}');
@@ -127434,15 +127475,15 @@
 INSERT INTO office_data VALUES('1138485','{"jis": "13105", "kana": "トウキヨウダイガクミナミケンキユウトウ", "name": "東京大学南研究棟", "prefecture": "東京都", "city": "文京区", "neighborhood": "本郷", "banchi": "7丁目3番1号", "postal_code": "1138485", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('1138555','{"jis": "13105", "kana": "トウキヨウトデンキキギヨウネンキンキキン", "name": "東京都電機企業年金基金", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "3丁目31番6号大塚ビルディング4階", "postal_code": "1138555", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138566','{"jis": "13105", "kana": "トウキヨウトデンキケンコウホケンクミアイ", "name": "東京都電機健康保険組合", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "3丁目15-4", "postal_code": "1138566", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138677','{"jis": "13105", "kana": "トウキヨウトリツコマゴメビヨウイン", "name": "東京都立駒込病院", "prefecture": "東京都", "city": "文京区", "neighborhood": "本駒込", "banchi": "3-18-22", "postal_code": "1138677", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンコマゴメ", "alternates": []}');
 INSERT INTO office_data VALUES('1138456','{"jis": "13105", "kana": "トウシバメデイカル カブシキガイシヤ", "name": "東芝メディカル　株式会社", "prefecture": "東京都", "city": "文京区", "neighborhood": "本郷", "banchi": "3丁目26-5", "postal_code": "1138456", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
 INSERT INTO office_data VALUES('1138513','{"jis": "13105", "kana": "トウホウレマツク カブシキガイシヤ", "name": "東邦レマック　株式会社", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "3丁目42-6", "postal_code": "1138513", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138435','{"jis": "13105", "kana": "トノクライカコウギヨウ カブシキガイシヤ", "name": "トノクラ医科工業　株式会社", "prefecture": "東京都", "city": "文京区", "neighborhood": "本郷", "banchi": "5丁目1-13", "postal_code": "1138435", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンゴウ", "alternates": []}');
-INSERT INTO office_data VALUES('1138663','{"jis": "13105", "kana": "ドクリツギヨウセイホウジン ジヨウホウシヨリスイシンキコウ アイテイ-ジンザイイクセイセンタ- コツカシカク・シケンブ", "name": "独立行政法人　情報処理推進機構　ＩＴ人材育成センター　国家資格・試験部", "prefecture": "東京都", "city": "文京区", "neighborhood": "本駒込", "banchi": "2丁目28-8文京グリーンコートセンターオフィス15階", "postal_code": "1138663", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンコマゴメ", "alternates": []}');
+INSERT INTO office_data VALUES('1138663','{"jis": "13105", "kana": "ドクリツギヨウセイホウジン ジヨウホウシヨリスイシンキコウ デジタルジンザイセンタ- コツカシカク・シケンブ", "name": "独立行政法人　情報処理推進機構　デジタル人材センター　国家資格・試験部", "prefecture": "東京都", "city": "文京区", "neighborhood": "本駒込", "banchi": "2丁目28-8文京グリーンコートセンターオフィス15階", "postal_code": "1138663", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンコマゴメ", "alternates": []}');
 INSERT INTO office_data VALUES('1138602','{"jis": "13105", "kana": "ニホンイカダイガク", "name": "日本医科大学", "prefecture": "東京都", "city": "文京区", "neighborhood": "千駄木", "banchi": "1丁目1-5", "postal_code": "1138602", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "センダギ", "alternates": []}');
 INSERT INTO office_data VALUES('1138603','{"jis": "13105", "kana": "ニホンイカダイガクフゾクビヨウイン", "name": "日本医科大学付属病院", "prefecture": "東京都", "city": "文京区", "neighborhood": "千駄木", "banchi": "1丁目1-5", "postal_code": "1138603", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "センダギ", "alternates": []}');
 INSERT INTO office_data VALUES('1138507','{"jis": "13105", "kana": "ニホンカナガタコウギヨウキギヨウネンキンキキン", "name": "日本金型工業企業年金基金", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "2-33-12", "postal_code": "1138507", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138610','{"jis": "13105", "kana": "ニホンコウギヨウシユツパン カブシキガイシヤ", "name": "日本工業出版　株式会社", "prefecture": "東京都", "city": "文京区", "neighborhood": "本駒込", "banchi": "6丁目3-26", "postal_code": "1138610", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンコマゴメ", "alternates": []}');
 INSERT INTO office_data VALUES('1138463','{"jis": "13105", "kana": "ニホンコクミンキユウエンカイ", "name": "日本国民救援会", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "2丁目4番4号", "postal_code": "1138463", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138441','{"jis": "13105", "kana": "ニホンシリツガツコウシンコウ・キヨウサイジギヨウダン", "name": "日本私立学校振興・共済事業団", "prefecture": "東京都", "city": "文京区", "neighborhood": "湯島", "banchi": "1丁目7-5", "postal_code": "1138441", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": true, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ユシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1138661','{"jis": "13105", "kana": "ニホンセイメイホケンソウゴガイシヤ", "name": "日本生命保険　相互会社", "prefecture": "東京都", "city": "文京区", "neighborhood": "本駒込", "banchi": "2丁目28-8", "postal_code": "1138661", "old_code": "113  ", "post_office": "本郷", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ブンキョウク", "neighborhood_kana": "ホンコマゴメ", "alternates": []}');
@@ -127532,15 +127573,15 @@
 INSERT INTO office_data VALUES('1108723','{"jis": "13106", "kana": "シヨウエイシヨクヒンコウギヨウ カブシキガイシヤ", "name": "正栄食品工業　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "秋葉原", "banchi": "5-7", "postal_code": "1108723", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アキハバラ", "alternates": []}');
 INSERT INTO office_data VALUES('1108576','{"jis": "13106", "kana": "シヨウワシツナイコウギヨウ (カブ)", "name": "昭和室内工業　（株）", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "5丁目23-11スグルビル6F", "postal_code": "1108576", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108620','{"jis": "13106", "kana": "シンメイワコウギヨウ カブシキガイシヤ パ-キングシステムジギヨウブ", "name": "新明和工業　株式会社　パーキングシステム事業部", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "5-16-5新明和上野ビル", "postal_code": "1108620", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108638','{"jis": "13106", "kana": "ジエイ・アキユレ-ト カブシキガイシヤ", "name": "ジェイ・アキュレート　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "6-27-5レジディア上野101", "postal_code": "1108638", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108618','{"jis": "13106", "kana": "ジエイ-ネツトチユウオウ カブシキガイシヤ", "name": "Ｊ－ＮＥＴ中央　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "1丁目6-2", "postal_code": "1108618", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108537','{"jis": "13106", "kana": "スズノヤ", "name": "（株）　鈴乃屋", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "1丁目20-11", "postal_code": "1108537", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108715','{"jis": "13106", "kana": "セイヨウケン", "name": "（株）　精養軒", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野公園", "banchi": "4-58", "postal_code": "1108715", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノコウエン", "alternates": []}');
-INSERT INTO office_data VALUES('1108646','{"jis": "13106", "kana": "ゼンコクインサツコウギヨウケンコウホケンクミアイ", "name": "全国印刷工業健康保険組合", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "1-7-2", "postal_code": "1108646", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
+INSERT INTO office_data VALUES('1108646','{"jis": "13106", "kana": "ゼンコクインサツコウギヨウケンコウホケンクミアイ", "name": "全国印刷工業健康保険組合", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "1-7-2", "postal_code": "1108646", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108722','{"jis": "13106", "kana": "ゼンコクシンブンジヨウホウノウギヨウ キヨウドウクミアイレンゴウカイ (ニホンノウギヨウシンブン)", "name": "全国新聞情報農業　協同組合連合会　（日本農業新聞）", "prefecture": "東京都", "city": "台東区", "neighborhood": "秋葉原", "banchi": "2-3", "postal_code": "1108722", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "アキハバラ", "alternates": []}');
 INSERT INTO office_data VALUES('1108628','{"jis": "13106", "kana": "ダイドウセイメイホケンソウゴガイシヤ", "name": "大同生命保険　相互会社　上野支社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "1丁目14-4上野三和ビル", "postal_code": "1108628", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108515','{"jis": "13106", "kana": "ダイワシヨウケン カブシキガイシヤ ウエノシテン", "name": "大和證券　株式会社　上野支店", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野", "banchi": "2丁目13-10", "postal_code": "1108515", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108635','{"jis": "13106", "kana": "チユウオウヒタチカデン カブシキガイシヤ", "name": "中央日立家電　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "東上野", "banchi": "2丁目7-5", "postal_code": "1108635", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ヒガシウエノ", "alternates": []}');
 INSERT INTO office_data VALUES('1108577','{"jis": "13106", "kana": "チヨダキコウ カブシキガイシヤ", "name": "千代田機工　株式会社", "prefecture": "東京都", "city": "台東区", "neighborhood": "台東", "banchi": "1丁目1-14", "postal_code": "1108577", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "タイトウ", "alternates": []}');
 INSERT INTO office_data VALUES('1108714','{"jis": "13106", "kana": "トウキヨウゲイジユツダイガク", "name": "東京芸術大学", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野公園", "banchi": "12-8", "postal_code": "1108714", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノコウエン", "alternates": []}');
 INSERT INTO office_data VALUES('1108712','{"jis": "13106", "kana": "トウキヨウコクリツハクブツカン", "name": "東京国立博物館", "prefecture": "東京都", "city": "台東区", "neighborhood": "上野公園", "banchi": "13-9", "postal_code": "1108712", "old_code": "110  ", "post_office": "上野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "タイトウク", "neighborhood_kana": "ウエノコウエン", "alternates": []}');
@@ -127769,14 +127810,15 @@
 INSERT INTO office_data VALUES('1358445','{"jis": "13108", "kana": "アサヒガラスホケンマネジメント カブシキガイシヤ", "name": "旭硝子保険マネジメント　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "2丁目31-1", "postal_code": "1358445", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358224','{"jis": "13108", "kana": "アスクル デイ-シ-エム ブツリユウセンタ-", "name": "アスクル　ＤＣＭ　物流センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "青海", "banchi": "4-1-16", "postal_code": "1358224", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "アオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358464','{"jis": "13108", "kana": "イツパンザイダンホウジン グリ-ンチヤンネル", "name": "一般財団法人　グリーンチャンネル", "prefecture": "東京都", "city": "江東区", "neighborhood": "永代", "banchi": "1丁目14番5号永代ダイヤビル13階", "postal_code": "1358464", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エイタイ", "alternates": []}');
 INSERT INTO office_data VALUES('1358411','{"jis": "13108", "kana": "イワノブツサン カブシキガイシヤ", "name": "岩野物産　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "東陽", "banchi": "4丁目1番7号佐藤ダイヤビルディング7階", "postal_code": "1358411", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トウヨウ", "alternates": []}');
 INSERT INTO office_data VALUES('1358318','{"jis": "13108", "kana": "インサツセイホンキカイケンコウホケンクミアイ", "name": "印刷製本包装機械健康保険組合", "prefecture": "東京都", "city": "江東区", "neighborhood": "毛利", "banchi": "2丁目6-5", "postal_code": "1358318", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "モウリ", "alternates": []}');
 INSERT INTO office_data VALUES('1358330','{"jis": "13108", "kana": "エイシンブツサン カブシキガイシヤ", "name": "栄進物産　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "森下", "banchi": "3丁目6-5", "postal_code": "1358330", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "モリシタ", "alternates": []}');
 INSERT INTO office_data VALUES('1358110','{"jis": "13108", "kana": "エスシ-エスケイ カブシキガイシヤ", "name": "ＳＣＳＫ　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "3丁目2番20号", "postal_code": "1358110", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
+INSERT INTO office_data VALUES('1358178','{"jis": "13108", "kana": "エヌ・テイ・テイ・デ-タ・カスタマサ-ビス カブシキガイシヤ", "name": "エヌ・ティ・ティ・データ・カスタマサービス　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "豊洲", "banchi": "3-3-9豊洲センタービルアネックス32F", "postal_code": "1358178", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "トヨス", "alternates": []}');
 INSERT INTO office_data VALUES('1358508','{"jis": "13108", "kana": "オ-ク カブシキガイシヤ", "name": "オーク　株式会社", "prefecture": "東京都", "city": "江東区", "neighborhood": "木場", "banchi": "6丁目3-2", "postal_code": "1358508", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "キバ", "alternates": []}');
 INSERT INTO office_data VALUES('1358558','{"jis": "13108", "kana": "オウジセイシ カブシキガイシヤ シノノメケンキユウセンタ-", "name": "王子製紙　株式会社　東雲研究センター", "prefecture": "東京都", "city": "江東区", "neighborhood": "東雲", "banchi": "1丁目10-6", "postal_code": "1358558", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シノノメ", "alternates": []}');
 INSERT INTO office_data VALUES('1358711','{"jis": "13108", "kana": "カエツアリアケチユウガツコウ・カエツアリアケコウトウガツコウ", "name": "かえつ有明中学校・かえつ有明高等学校", "prefecture": "東京都", "city": "江東区", "neighborhood": "東雲", "banchi": "2丁目16-1", "postal_code": "1358711", "old_code": "135  ", "post_office": "晴海", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シノノメ", "alternates": []}');
 INSERT INTO office_data VALUES('1358565','{"jis": "13108", "kana": "カテナ カブシキガイシヤ", "name": "カテナ　（株）", "prefecture": "東京都", "city": "江東区", "neighborhood": "潮見", "banchi": "2丁目10-24", "postal_code": "1358565", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シオミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358517','{"jis": "13108", "kana": "カブ) スポ-ツニツポンシンブン トウキヨウホンシヤ", "name": "（株）　スポーツニッポン新聞　東京本社", "prefecture": "東京都", "city": "江東区", "neighborhood": "越中島", "banchi": "2丁目1-30", "postal_code": "1358517", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "エッチュウジマ", "alternates": []}');
 INSERT INTO office_data VALUES('1358556','{"jis": "13108", "kana": "カブ) トウキヨウウサミ", "name": "（株）　東京宇佐美", "prefecture": "東京都", "city": "江東区", "neighborhood": "辰巳", "banchi": "1丁目7-17", "postal_code": "1358556", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "タツミ", "alternates": []}');
 INSERT INTO office_data VALUES('1358350','{"jis": "13108", "kana": "カブ) トウキヨウクラウン", "name": "（株）　東京クラウン", "prefecture": "東京都", "city": "江東区", "neighborhood": "新大橋", "banchi": "2丁目13-4", "postal_code": "1358350", "old_code": "135  ", "post_office": "深川", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "コウトウク", "neighborhood_kana": "シンオオハシ", "alternates": []}');
@@ -128088,15 +128130,14 @@
 INSERT INTO office_data VALUES('1418501','{"jis": "13109", "kana": "アルパイン カブシキガイシヤ", "name": "アルパイン　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "1丁目1-8大手町建物ビル", "postal_code": "1418501", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418522','{"jis": "13109", "kana": "イトウチユウテクノソリユ-シヨンズ (カブ) オオサキオフイス", "name": "伊藤忠テクノソリューションズ　（株）　大崎オフィス", "prefecture": "東京都", "city": "品川区", "neighborhood": "大崎", "banchi": "1丁目2-2", "postal_code": "1418522", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('1418658','{"jis": "13109", "kana": "イノウエデンキ カブシキガイシヤ", "name": "井上電気　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "上大崎", "banchi": "3丁目14-12", "postal_code": "1418658", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "カミオオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('1418646','{"jis": "13109", "kana": "オオサキデンキコウギヨウ カブシキガイシヤ", "name": "大崎電気工業　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "東五反田", "banchi": "2丁目10-2東五反田スクエア", "postal_code": "1418646", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ヒガシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418517','{"jis": "13109", "kana": "オサダデンキコウギヨウ カブシキガイシヤ", "name": "長田電機工業　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "5丁目17-5", "postal_code": "1418517", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418525','{"jis": "13109", "kana": "オザワブツサン カブシキカイシヤ", "name": "小澤物産　株式会社", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "7丁目24番5号", "postal_code": "1418525", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418580','{"jis": "13109", "kana": "カブシキガイシヤ アオイ プロ", "name": "株式会社　ＡＯＩ　Ｐｒｏ．", "prefecture": "東京都", "city": "品川区", "neighborhood": "大崎", "banchi": "1丁目5-1大崎センタービル", "postal_code": "1418580", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオサキ", "alternates": []}');
-INSERT INTO office_data VALUES('1058711','{"jis": "13109", "kana": "カブシキガイシヤ エツクスワン", "name": "株式会社　エックスワン", "prefecture": "東京都", "city": "品川区", "neighborhood": "大崎", "banchi": "1丁目11-2(芝郵便局私書箱第211号)", "postal_code": "1058711", "old_code": "141  ", "post_office": "芝", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "オオサキ", "alternates": []}');
 INSERT INTO office_data VALUES('1098792','{"jis": "13109", "kana": "カブシキガイシヤ カンポセイメイホケン トウキヨウサ-ビスセンタ-", "name": "株式会社　かんぽ生命保険　東京サービスセンター", "prefecture": "東京都", "city": "品川区", "neighborhood": "北品川", "banchi": "5丁目6-1大崎ブライトタワー", "postal_code": "1098792", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "キタシナガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1418416','{"jis": "13109", "kana": "カブシキガイシヤ ガツケン", "name": "株式会社　Ｇａｋｋｅｎ", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "2-11-8", "postal_code": "1418416", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418422','{"jis": "13109", "kana": "カブシキガイシヤ ガツケンアソシエ", "name": "株式会社　学研アソシエ", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "8-1-13タケウチビル4F", "postal_code": "1418422", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418411','{"jis": "13109", "kana": "カブシキガイシヤ ガツケンエデユケ-シヨナル", "name": "株式会社　学研エデュケーショナル", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "2-11-8", "postal_code": "1418411", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418424','{"jis": "13109", "kana": "カブシキガイシヤ ガツケンキヨウイクアイ・シ-・テイ-", "name": "株式会社　学研教育アイ・シー・ティー", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "2-11-8", "postal_code": "1418424", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418413','{"jis": "13109", "kana": "カブシキガイシヤ ガツケンキヨウイクシユツパン", "name": "株式会社　学研教育出版", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "2-11-8", "postal_code": "1418413", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
 INSERT INTO office_data VALUES('1418420','{"jis": "13109", "kana": "カブシキガイシヤ ガツケンココフアンホ-ルデイングス", "name": "株式会社　学研ココファンホールディングス", "prefecture": "東京都", "city": "品川区", "neighborhood": "西五反田", "banchi": "2-11-8", "postal_code": "1418420", "old_code": "141  ", "post_office": "大崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "シナガワク", "neighborhood_kana": "ニシゴタンダ", "alternates": []}');
@@ -128996,15 +129037,15 @@
 INSERT INTO office_data VALUES('1148571','{"jis": "13117", "kana": "タキノガワシンヨウキンコ", "name": "瀧野川信用金庫", "prefecture": "東京都", "city": "北区", "neighborhood": "田端新町", "banchi": "3丁目25-2", "postal_code": "1148571", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "タバタシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1148540','{"jis": "13117", "kana": "タツミサンギヨウ カブシキガイシヤ", "name": "タツミ産業　株式会社", "prefecture": "東京都", "city": "北区", "neighborhood": "上十条", "banchi": "2丁目13-1", "postal_code": "1148540", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "カミジュウジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1148523','{"jis": "13117", "kana": "タバタブンシムラキネンカン", "name": "田端文士村記念館", "prefecture": "東京都", "city": "北区", "neighborhood": "田端", "banchi": "6-1-2田端ASUKAタワー内", "postal_code": "1148523", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "タバタ", "alternates": []}');
 INSERT INTO office_data VALUES('1148686','{"jis": "13117", "kana": "チユウオウコウガツコウ シヨウガイガクシユウセンタ-", "name": "中央工学校　生涯学習センター", "prefecture": "東京都", "city": "北区", "neighborhood": "中里", "banchi": "1丁目15-7", "postal_code": "1148686", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ナカザト", "alternates": []}');
 INSERT INTO office_data VALUES('1148545','{"jis": "13117", "kana": "ト-メンシヨクヒン カブシキガイシヤ", "name": "トーメン食品　株式会社", "prefecture": "東京都", "city": "北区", "neighborhood": "十条台", "banchi": "1丁目4-15", "postal_code": "1148545", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ジュウジョウダイ", "alternates": []}');
 INSERT INTO office_data VALUES('1148539','{"jis": "13117", "kana": "トウカイシヨウジ カブシキガイシヤ", "name": "東海商事　株式会社", "prefecture": "東京都", "city": "北区", "neighborhood": "東田端", "banchi": "2丁目4-4", "postal_code": "1148539", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ヒガシタバタ", "alternates": []}');
 INSERT INTO office_data VALUES('1148580','{"jis": "13117", "kana": "トウキヨウガイコクゴダイガク", "name": "東京外国語大学", "prefecture": "東京都", "city": "北区", "neighborhood": "西ケ原", "banchi": "4丁目51-21", "postal_code": "1148580", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ニシガハラ", "alternates": []}');
-INSERT INTO office_data VALUES('1148535','{"jis": "13117", "kana": "トウキヨウガス ホクブジギヨウホンブ", "name": "東京ガス　（株）　北部事業本部", "prefecture": "東京都", "city": "北区", "neighborhood": "滝野川", "banchi": "5丁目42", "postal_code": "1148535", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "タキノガワ", "alternates": []}');
+INSERT INTO office_data VALUES('1148535','{"jis": "13117", "kana": "トウキヨウガスネツトワ-ク (カブ)", "name": "東京ガスネットワーク　（株）", "prefecture": "東京都", "city": "北区", "neighborhood": "滝野川", "banchi": "5-42", "postal_code": "1148535", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "タキノガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1148524','{"jis": "13117", "kana": "トウキヨウシヨセキ カブシキガイシヤ", "name": "東京書籍　株式会社", "prefecture": "東京都", "city": "北区", "neighborhood": "堀船", "banchi": "2丁目17-1", "postal_code": "1148524", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ホリフネ", "alternates": []}');
 INSERT INTO office_data VALUES('1148526','{"jis": "13117", "kana": "トウキヨウセイトクガクエン", "name": "学校法人　東京成徳学園", "prefecture": "東京都", "city": "北区", "neighborhood": "豊島", "banchi": "8丁目26-9", "postal_code": "1148526", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "トシマ", "alternates": []}');
 INSERT INTO office_data VALUES('1148508','{"jis": "13117", "kana": "トウキヨウトキタクヤクシヨ", "name": "東京都北区役所", "prefecture": "東京都", "city": "北区", "neighborhood": "王子本町", "banchi": "1丁目15-22", "postal_code": "1148508", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "オウジホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1148546','{"jis": "13117", "kana": "トウキヨウトキタクヤクシヨ タキノガワブンチヨウシヤ", "name": "東京都北区役所　滝野川分庁舎", "prefecture": "東京都", "city": "北区", "neighborhood": "滝野川", "banchi": "2-52-10", "postal_code": "1148546", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "タキノガワ", "alternates": []}');
 INSERT INTO office_data VALUES('1148517','{"jis": "13117", "kana": "トウキヨウトキタトゼイジムシヨ", "name": "東京都北都税事務所", "prefecture": "東京都", "city": "北区", "neighborhood": "中十条", "banchi": "1丁目7-8", "postal_code": "1148517", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "ナカジュウジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1148506','{"jis": "13117", "kana": "トウキヨウトスイドウキヨク キタエイギヨウシヨ", "name": "東京都水道局　北営業所", "prefecture": "東京都", "city": "北区", "neighborhood": "上十条", "banchi": "1丁目9-17", "postal_code": "1148506", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "カミジュウジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1148561','{"jis": "13117", "kana": "トウキヨウトリツ アスカコウトウガツコウ", "name": "東京都立　飛鳥高等学校", "prefecture": "東京都", "city": "北区", "neighborhood": "王子", "banchi": "6丁目8-8", "postal_code": "1148561", "old_code": "114  ", "post_office": "王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "キタク", "neighborhood_kana": "オウジ", "alternates": []}');
@@ -129375,15 +129416,15 @@
 INSERT INTO office_data VALUES('1928568','{"jis": "13201", "kana": "トウキヨウトリツハチオウジヒガシコウトウガツコウ", "name": "東京都立八王子東高等学校", "prefecture": "東京都", "city": "八王子市", "neighborhood": "高倉町", "banchi": "68番1", "postal_code": "1928568", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "タカクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1928562','{"jis": "13201", "kana": "トウキヨウトリツミナミタマチユウトウキヨウイクガツコウ", "name": "東京都立南多摩中等教育学校", "prefecture": "東京都", "city": "八王子市", "neighborhood": "明神町", "banchi": "4-20-1", "postal_code": "1928562", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ミョウジンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1928648','{"jis": "13201", "kana": "ナカニホンコウソクドウロ カブシキガイシヤ ハチオウジシシヤ", "name": "中日本高速道路　（株）　八王子支社", "prefecture": "東京都", "city": "八王子市", "neighborhood": "宇津木町", "banchi": "231", "postal_code": "1928648", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ウツキマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1920988','{"jis": "13201", "kana": "ニツポンスイサン カブシキカイシヤ ハチオウジソウゴウコウジヨウ", "name": "日本水産　株式会社　八王子総合工場", "prefecture": "東京都", "city": "八王子市", "neighborhood": "北野町", "banchi": "559-6番地", "postal_code": "1920988", "old_code": "192  ", "post_office": "八王子南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "キタノマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1928644','{"jis": "13201", "kana": "ニホンギンシワ-ム", "name": "日本銀刺ワーム", "prefecture": "東京都", "city": "八王子市", "neighborhood": "明神町", "banchi": "3丁目26-1", "postal_code": "1928644", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ミョウジンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1920983','{"jis": "13201", "kana": "ニホンコウガクインハチオウジセンモンガツコウ", "name": "日本工学院八王子専門学校", "prefecture": "東京都", "city": "八王子市", "neighborhood": "片倉町", "banchi": "1404番1号", "postal_code": "1920983", "old_code": "192  ", "post_office": "八王子南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "カタクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1928633','{"jis": "13201", "kana": "ニホンコンテツク カブシキガイシヤ サンギヨウシザイブ", "name": "日本コンテック　株式会社　産業資材部", "prefecture": "東京都", "city": "八王子市", "neighborhood": "小門町", "banchi": "53番地", "postal_code": "1928633", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "オカドマチ", "alternates": []}');
-INSERT INTO office_data VALUES('1928585','{"jis": "13201", "kana": "ニホンヒユ-レツト・パツカ-ド カブシキガイシヤ ハチオウジジギヨウシヨ", "name": "日本ヒューレット・パッカード　株式会社　八王子事業所", "prefecture": "東京都", "city": "八王子市", "neighborhood": "明神町", "banchi": "4丁目9-8", "postal_code": "1928585", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ミョウジンチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('1928585','{"jis": "13201", "kana": "ニホンヒユ-レツト・パツカ-ド ゴウドウカイシヤ", "name": "日本ヒューレット・パッカード　合同会社", "prefecture": "東京都", "city": "八王子市", "neighborhood": "東町", "banchi": "9-8八王子東町センタービル2F", "postal_code": "1928585", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "アズマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1920986','{"jis": "13201", "kana": "ニホンブンカダイガク", "name": "日本文化大學", "prefecture": "東京都", "city": "八王子市", "neighborhood": "片倉町", "banchi": "977番地", "postal_code": "1920986", "old_code": "192  ", "post_office": "八王子南", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "カタクラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1928537','{"jis": "13201", "kana": "ニホンブンコウ カブシキガイシヤ", "name": "日本分光　株式会社", "prefecture": "東京都", "city": "八王子市", "neighborhood": "石川町", "banchi": "2967-5", "postal_code": "1928537", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "イシカワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('1928516','{"jis": "13201", "kana": "ハチオウジカンイサイバンシヨ", "name": "八王子簡易裁判所", "prefecture": "東京都", "city": "八王子市", "neighborhood": "明神町", "banchi": "4丁目21-1", "postal_code": "1928516", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ミョウジンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1928506','{"jis": "13201", "kana": "ハチオウジシヤカイホケンジムシヨ", "name": "八王子社会保険事務所", "prefecture": "東京都", "city": "八王子市", "neighborhood": "南新町", "banchi": "4-1", "postal_code": "1928506", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "ミナミシンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1928501','{"jis": "13201", "kana": "ハチオウジシヤクシヨ", "name": "八王子市役所", "prefecture": "東京都", "city": "八王子市", "neighborhood": "元本郷町", "banchi": "3丁目24-1", "postal_code": "1928501", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "モトホンゴウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1928702','{"jis": "13201", "kana": "ハチオウジシヤクシヨ シミンブシミンカ", "name": "八王子市役所　市民部市民課", "prefecture": "東京都", "city": "八王子市", "neighborhood": "元本郷町", "banchi": "3丁目24-1(八王子郵便局私書箱第2号)", "postal_code": "1928702", "old_code": "192  ", "post_office": "八王子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "モトホンゴウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('1928520','{"jis": "13201", "kana": "ハチオウジシヨウコウカイギシヨ", "name": "八王子商工会議所", "prefecture": "東京都", "city": "八王子市", "neighborhood": "大横町", "banchi": "11-1", "postal_code": "1928520", "old_code": "192  ", "post_office": "八王子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トウキョウト", "city_kana": "ハチオウジシ", "neighborhood_kana": "オオヨコチョウ", "alternates": []}');
@@ -129994,14 +130035,15 @@
 INSERT INTO office_data VALUES('2318772','{"jis": "14104", "kana": "ヨコハマシコドモセイシヨウネンキヨク コドモカテイカ", "name": "横浜市こども青少年局　こども家庭課", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "桜木町", "banchi": "1-1-56みなとみらい21クリーンセンター5階", "postal_code": "2318772", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318771','{"jis": "14104", "kana": "ヨコハマシコドモセイシヨウネンキヨク コドモカテイカ", "name": "横浜市こども青少年局　こども家庭課", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "桜木町", "banchi": "1-1-56みなとみらい21クリーンセンター5階", "postal_code": "2318771", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318343','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ シヨウキヤクシサンカ", "name": "横浜市財政局主税部　償却資産課", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318343", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318313','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ノウゼイカンリカ", "name": "横浜市財政局主税部　納税管理課", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318313", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318312','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ ジギヨウシヨゼイタントウ", "name": "横浜市財政局主税部　法人課税課　事業所税担当", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318312", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318314','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ トクベツチヨウシユウセンタ-", "name": "横浜市財政局主税部　法人課税課　特別徴収センター", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318314", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318316','{"jis": "14104", "kana": "ヨコハマシザイセイキヨクシユゼイブ ホウジンカゼイカ ホウジンシミンゼイタントウ", "name": "横浜市財政局主税部　法人課税課　法人市民税担当", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山下町", "banchi": "2", "postal_code": "2318316", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマシタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('2318455','{"jis": "14104", "kana": "ヨコハマシシミンブンカカイカンカンナイホ-ル", "name": "横浜市市民文化会館関内ホール", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "住吉町", "banchi": "4-42-1", "postal_code": "2318455", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": true, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "スミヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318307','{"jis": "14104", "kana": "ヨコハマシユウソウセイキユウジムセンタ-", "name": "横浜市郵送請求事務センター", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "桜木町", "banchi": "1丁目1-56", "postal_code": "2318307", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318682','{"jis": "14104", "kana": "ヨコハマシリツ ミナトセキジユウジビヨウイン", "name": "横浜市立　みなと赤十字病院", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新山下", "banchi": "3丁目12-1", "postal_code": "2318682", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンヤマシタ", "alternates": []}');
 INSERT INTO office_data VALUES('2318411','{"jis": "14104", "kana": "ヨコハマチホウホウムキヨク", "name": "横浜地方法務局", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "北仲通", "banchi": "5丁目57横浜第2合同庁舎", "postal_code": "2318411", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "キタナカドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('2318750','{"jis": "14104", "kana": "ヨコハマナカゼイムシヨ", "name": "横浜中税務署", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新港", "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階", "postal_code": "2318750", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンコウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318550','{"jis": "14104", "kana": "ヨコハマナカゼイムシヨ", "name": "横浜中税務署", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "新港", "banchi": "一丁目6番1号よこはま新港合同庁舎2階・3階", "postal_code": "2318550", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": true, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "シンコウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318562','{"jis": "14104", "kana": "ヨコハマフタバシヨウガツコウ", "name": "横浜雙葉小学校", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "山手町", "banchi": "226", "postal_code": "2318562", "old_code": "231  ", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ヤマテチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2318689','{"jis": "14104", "kana": "ヨシカワシヨウジ カブシキカイシヤ", "name": "吉川商事　株式会社", "prefecture": "神奈川県", "city": "横浜市中区", "neighborhood": "上野町", "banchi": "2丁目88番地", "postal_code": "2318689", "old_code": "23108", "post_office": "横浜港", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "ヨコハマシナカク", "neighborhood_kana": "ウエノチョウ", "alternates": []}');
@@ -130419,15 +130461,14 @@
 INSERT INTO office_data VALUES('2525287','{"jis": "14152", "kana": "トウプレ カブシキガイシヤ サガミハラジギヨウシヨ", "name": "東プレ　株式会社　相模原事業所", "prefecture": "神奈川県", "city": "相模原市中央区", "neighborhood": "南橋本", "banchi": "3丁目2-25", "postal_code": "2525287", "old_code": "25252", "post_office": "相模原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシチュウオウク", "neighborhood_kana": "ミナミハシモト", "alternates": []}');
 INSERT INTO office_data VALUES('2525250','{"jis": "14152", "kana": "ニホンルメンタム カブシキガイシヤ", "name": "日本ルメンタム　株式会社", "prefecture": "神奈川県", "city": "相模原市中央区", "neighborhood": "小山", "banchi": "4-1-55", "postal_code": "2525250", "old_code": "25252", "post_office": "相模原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシチュウオウク", "neighborhood_kana": "オヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('2525297','{"jis": "14152", "kana": "マイクロンハシモトギジユツセンタ-", "name": "マイクロン橋本技術センター", "prefecture": "神奈川県", "city": "相模原市中央区", "neighborhood": "南橋本", "banchi": "3丁目1番35号", "postal_code": "2525297", "old_code": "25252", "post_office": "相模原", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシチュウオウク", "neighborhood_kana": "ミナミハシモト", "alternates": []}');
 INSERT INTO office_data VALUES('2520370','{"jis": "14153", "kana": "カブシキカイシヤ ヨコハマオカダヤ", "name": "株式会社　横浜岡田屋", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "相模大野", "banchi": "3丁目9-1", "postal_code": "2520370", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "サガミオオノ", "alternates": []}');
 INSERT INTO office_data VALUES('2520373','{"jis": "14153", "kana": "ガツコウホウジン キタサトケンキユウシヨ", "name": "学校法人　北里研究所", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "北里", "banchi": "1丁目15-1", "postal_code": "2520373", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "キタザト", "alternates": []}');
 INSERT INTO office_data VALUES('2520383','{"jis": "14153", "kana": "ガツコウホウジン サガミジヨシダイガク", "name": "学校法人　相模女子大学", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "文京", "banchi": "2丁目1-1", "postal_code": "2520383", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "ブンキョウ", "alternates": []}');
 INSERT INTO office_data VALUES('2520374','{"jis": "14153", "kana": "キタサトダイガク イガクブ", "name": "北里大学　医学部", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "北里", "banchi": "1丁目15番1号", "postal_code": "2520374", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "キタザト", "alternates": []}');
-INSERT INTO office_data VALUES('2520380','{"jis": "14153", "kana": "キタサトダイガクヒガシビヨウイン", "name": "北里大学東病院", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "麻溝台", "banchi": "2丁目1-1", "postal_code": "2520380", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "アサミゾダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2520375','{"jis": "14153", "kana": "キタサトダイガクビヨウイン", "name": "北里大学病院", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "北里", "banchi": "1丁目15番1号", "postal_code": "2520375", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "キタザト", "alternates": []}');
 INSERT INTO office_data VALUES('2520381','{"jis": "14153", "kana": "サガミハラケンゼイジムシヨ", "name": "相模原県税事務所", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "相模大野", "banchi": "6丁目3-1", "postal_code": "2520381", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "サガミオオノ", "alternates": []}');
 INSERT INTO office_data VALUES('2520377','{"jis": "14153", "kana": "サガミハラシ ミナミクヤクシヨ", "name": "相模原市　南区役所", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "相模大野", "banchi": "5丁目31番1号南区合同庁舎内", "postal_code": "2520377", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "サガミオオノ", "alternates": []}');
 INSERT INTO office_data VALUES('2520388','{"jis": "14153", "kana": "サガミハラネンキンジムシヨ", "name": "相模原年金事務所", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "相模大野", "banchi": "6丁目6-6", "postal_code": "2520388", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "サガミオオノ", "alternates": []}');
 INSERT INTO office_data VALUES('2528538','{"jis": "14153", "kana": "ジヨシビジユツダイガク", "name": "女子美術大学", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "麻溝台", "banchi": "1900", "postal_code": "2528538", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "アサミゾダイ", "alternates": []}');
 INSERT INTO office_data VALUES('2520395','{"jis": "14153", "kana": "トウカイダイガクフゾクサガミコウトウガツコウ・チユウトウブ", "name": "東海大学付属相模高等学校・中等部", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "相南", "banchi": "3丁目33-1", "postal_code": "2520395", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "ソウナン", "alternates": []}');
 INSERT INTO office_data VALUES('2520385','{"jis": "14153", "kana": "トウシバリンカンビヨウイン", "name": "東芝林間病院", "prefecture": "神奈川県", "city": "相模原市南区", "neighborhood": "上鶴間", "banchi": "7丁目9-1", "postal_code": "2520385", "old_code": "228  ", "post_office": "座間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "カナガワケン", "city_kana": "サガミハラシミナミク", "neighborhood_kana": "カミツルマ", "alternates": []}');
@@ -130684,14 +130725,15 @@
 INSERT INTO office_data VALUES('9503198','{"jis": "15101", "kana": "ニイガタイリヨウフクシダイガク", "name": "新潟医療福祉大学", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "島見町", "banchi": "1398番地", "postal_code": "9503198", "old_code": "95031", "post_office": "松浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "シマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9503197','{"jis": "15101", "kana": "ニイガタシヨクリヨウノウギヨウダイガク ニイガタキヤンパス", "name": "新潟食料農業大学　新潟キャンパス", "prefecture": "新潟県", "city": "新潟市北区", "neighborhood": "島見町", "banchi": "940番地", "postal_code": "9503197", "old_code": "95031", "post_office": "松浜", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシキタク", "neighborhood_kana": "シマミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508735','{"jis": "15102", "kana": "イチマサカマボコ カブシキガイシヤ", "name": "一正蒲鉾　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "津島屋", "banchi": "7丁目77", "postal_code": "9508735", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "ツシマヤ", "alternates": []}');
 INSERT INTO office_data VALUES('9508723','{"jis": "15102", "kana": "イデミツコウサン カブシキガイシヤ ニイガタセキユセイヒンユニユウキチ", "name": "出光興産　株式会社　新潟石油製品輸入基地", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "臨港町", "banchi": "3丁目4914番479", "postal_code": "9508723", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "リンコウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508640','{"jis": "15102", "kana": "カブシキガイシヤ ダイヤメツト", "name": "株式会社　ダイヤメット", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "小金町", "banchi": "3丁目1番1号", "postal_code": "9508640", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "コガネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508715','{"jis": "15102", "kana": "カブシキガイシヤ ナビツク", "name": "株式会社　ナビック", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "松島", "banchi": "1丁目2-8", "postal_code": "9508715", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "マツシマ", "alternates": []}');
 INSERT INTO office_data VALUES('9508707','{"jis": "15102", "kana": "カブシキガイシヤ ニイガタヒタチ", "name": "株式会社　新潟日立", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "竹尾卸新町", "banchi": "752-10", "postal_code": "9508707", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "タケオオロシシンマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9508701','{"jis": "15102", "kana": "クロスウイルメデイカル カブシキガイシヤ", "name": "クロスウィルメディカル　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "紫竹卸新町", "banchi": "1808番地22", "postal_code": "9508701", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "シチクオロシシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9508680','{"jis": "15102", "kana": "コウリツダイガクホウジン ニイガタケンリツダイガク", "name": "公立大学法人　新潟県立大学", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "海老ケ瀬", "banchi": "471", "postal_code": "9508680", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "エビガセ", "alternates": []}');
 INSERT INTO office_data VALUES('9508730','{"jis": "15102", "kana": "サトウシヨクヒン カブシキガイシヤ", "name": "サトウ食品　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "宝町", "banchi": "13-5", "postal_code": "9508730", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "タカラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9508725','{"jis": "15102", "kana": "シヤカイイリヨウホウジン ニイガタリンコウホケンカイ ニイガタリンコウビヨウイン", "name": "社会医療法人　新潟臨港保健会　新潟臨港病院", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "桃山町", "banchi": "1丁目114番地3", "postal_code": "9508725", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "モモヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508720','{"jis": "15102", "kana": "シロセシヨウジ カブシキガイシヤ", "name": "白勢商事　株式会社", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "山木戸", "banchi": "8丁目8-1", "postal_code": "9508720", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "ヤマキド", "alternates": []}');
 INSERT INTO office_data VALUES('9508678','{"jis": "15102", "kana": "ジヤスコ カブシキガイシヤ ニイガタヒガシシテン", "name": "ジャスコ　株式会社　新潟東支店", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "大形本町", "banchi": "3丁目1-2", "postal_code": "9508678", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "オオガタホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508744','{"jis": "15102", "kana": "トウホクデンリヨク カブシキガイシヤ ニイガタカリヨクハツデンシヨ", "name": "東北電力　株式会社　新潟火力発電所", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "桃山町", "banchi": "2丁目200", "postal_code": "9508744", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "モモヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9508639','{"jis": "15102", "kana": "ニイガタケンリツ ニイガタヒガシコウトウガツコウ", "name": "新潟県立　新潟東高等学校", "prefecture": "新潟県", "city": "新潟市東区", "neighborhood": "小金町", "banchi": "2丁目6-1", "postal_code": "9508639", "old_code": "950  ", "post_office": "新潟中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ニイガタシヒガシク", "neighborhood_kana": "コガネチョウ", "alternates": []}');
@@ -131002,15 +131044,17 @@
 INSERT INTO office_data VALUES('9402085','{"jis": "15202", "kana": "ナガオカセキジユウジビヨウイン", "name": "長岡赤十字病院", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "千秋", "banchi": "2丁目297-1", "postal_code": "9402085", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "センシュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9402088','{"jis": "15202", "kana": "ナガオカゾウケイダイガク", "name": "長岡造形大学", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "千秋", "banchi": "4丁目197", "postal_code": "9402088", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "センシュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9402081','{"jis": "15202", "kana": "ナガオカニシビヨウイン", "name": "長岡西病院", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "三ツ郷屋町", "banchi": "371-1", "postal_code": "9402081", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9402083','{"jis": "15202", "kana": "ニイガタケンリツ キンダイビジユツカン", "name": "新潟県立　近代美術館", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "千秋", "banchi": "3丁目278-14", "postal_code": "9402083", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "センシュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9402184','{"jis": "15202", "kana": "ニイガタケンリツナガオカコウリヨウコウトウガツコウ", "name": "新潟県立長岡向陵高等学校", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "喜多町", "banchi": "1030-1", "postal_code": "9402184", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "キタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9402093','{"jis": "15202", "kana": "リバ-サイドセンシユウ アピタ・モ-ル", "name": "リバーサイド千秋　アピタ・モール", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "千秋", "banchi": "2丁目278番地", "postal_code": "9402093", "old_code": "94021", "post_office": "長岡西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "センシュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9402392','{"jis": "15202", "kana": "ナガオカシヤクシヨ ミシマシシヨ", "name": "長岡市役所　三島支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "上岩井", "banchi": "1261-1", "postal_code": "9402392", "old_code": "94023", "post_office": "脇野町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "カミイワイ", "alternates": []}');
+INSERT INTO office_data VALUES('9402492','{"jis": "15202", "kana": "ナガオカシヤクシヨヨイタシシヨ", "name": "長岡市役所与板支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "与板町与板", "banchi": "甲134番地", "postal_code": "9402492", "old_code": "94024", "post_office": "与板", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ヨイタマチヨイタ", "alternates": []}');
 INSERT INTO office_data VALUES('9402595','{"jis": "15202", "kana": "カクジヨウギヨルイホ-ルデイングス カブシキガイシヤ", "name": "角上魚類ホールディングス　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "寺泊", "banchi": "下荒町9772-20", "postal_code": "9402595", "old_code": "94025", "post_office": "寺泊", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "テラドマリ", "alternates": []}');
+INSERT INTO office_data VALUES('9402592','{"jis": "15202", "kana": "ナガオカシヤクシヨテラドマリシシヨ", "name": "長岡市役所寺泊支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "寺泊", "banchi": "鳥帽子平1977番地8", "postal_code": "9402592", "old_code": "94025", "post_office": "寺泊", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "テラドマリ", "alternates": []}');
 INSERT INTO office_data VALUES('9495292','{"jis": "15202", "kana": "ナガオカシヤクシヨ オグニシシヨ", "name": "長岡市役所　小国支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "小国町法坂", "banchi": "793", "postal_code": "9495292", "old_code": "94952", "post_office": "七日町", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "オグニマチホウザカ", "alternates": []}');
 INSERT INTO office_data VALUES('9495494','{"jis": "15202", "kana": "アサヒシユゾウ カブシキガイシヤ", "name": "朝日酒造　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "朝日", "banchi": "880-1", "postal_code": "9495494", "old_code": "94954", "post_office": "来迎寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "アサヒ", "alternates": []}');
 INSERT INTO office_data VALUES('9495492','{"jis": "15202", "kana": "イワツカセイカ カブシキガイシヤ", "name": "岩塚製菓　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "飯塚", "banchi": "2958番地", "postal_code": "9495492", "old_code": "94954", "post_office": "来迎寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "イイヅカ", "alternates": []}');
 INSERT INTO office_data VALUES('9495493','{"jis": "15202", "kana": "ナガオカシヤクシヨ コシジシシヨ", "name": "長岡市役所　越路支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "浦", "banchi": "715", "postal_code": "9495493", "old_code": "94954", "post_office": "来迎寺", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ウラ", "alternates": []}');
 INSERT INTO office_data VALUES('9497594','{"jis": "15202", "kana": "シンエツコウギヨウ カブシキガイシヤ", "name": "信越工業　株式会社", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "西川口", "banchi": "528番地", "postal_code": "9497594", "old_code": "94975", "post_office": "川口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ニシカワグチ", "alternates": []}');
 INSERT INTO office_data VALUES('9497592','{"jis": "15202", "kana": "ナガオカシヤクシヨ カワグチシシヨ", "name": "長岡市役所　川口支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "東川口", "banchi": "1974-26", "postal_code": "9497592", "old_code": "94975", "post_office": "川口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ヒガシカワグチ", "alternates": []}');
 INSERT INTO office_data VALUES('9540192','{"jis": "15202", "kana": "ナガオカシヤクシヨ ナカノシマシシヨ", "name": "長岡市役所　中之島支所", "prefecture": "新潟県", "city": "長岡市", "neighborhood": "中之島", "banchi": "788(今町郵便局私書箱第8号)", "postal_code": "9540192", "old_code": "95401", "post_office": "見附", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ニイガタケン", "city_kana": "ナガオカシ", "neighborhood_kana": "ナカノシマ", "alternates": []}');
@@ -131886,19 +131930,19 @@
 INSERT INTO office_data VALUES('9238570','{"jis": "17203", "kana": "コマツゼイムシヨ", "name": "小松税務署", "prefecture": "石川県", "city": "小松市", "neighborhood": "日の出町", "banchi": "1丁目120", "postal_code": "9238570", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ヒノデマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238642','{"jis": "17203", "kana": "コマツデンシ カブシキガイシヤ", "name": "小松電子　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "安宅町", "banchi": "甲135", "postal_code": "9238642", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "アタカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238502','{"jis": "17203", "kana": "コマニ- カブシキガイシヤ", "name": "コマニー　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "工業団地", "banchi": "1丁目93番地", "postal_code": "9238502", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "コウギョウダンチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238610','{"jis": "17203", "kana": "サイエンスヒルズコマツ", "name": "サイエンスヒルズこまつ", "prefecture": "石川県", "city": "小松市", "neighborhood": "こまつの杜", "banchi": "2番地", "postal_code": "9238610", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "コマツノモリ", "alternates": []}');
 INSERT INTO office_data VALUES('9238630','{"jis": "17203", "kana": "ザイダンホウジン コマツカンゴガツコウ", "name": "財団法人　こまつ看護学校", "prefecture": "石川県", "city": "小松市", "neighborhood": "向本折町", "banchi": "ヘ14-1", "postal_code": "9238630", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ムカイモトオリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238616','{"jis": "17203", "kana": "シノオカケンセツ カブシキガイシヤ", "name": "篠岡建設　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "桜木町", "banchi": "133-1", "postal_code": "9238616", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "サクラギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9238575','{"jis": "17203", "kana": "ジエイ・バス カブシキガイシヤ", "name": "ジェイ・バス　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "串町", "banchi": "工業団地30番地", "postal_code": "9238575", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "クシマチ", "alternates": []}');
-INSERT INTO office_data VALUES('9238552','{"jis": "17203", "kana": "セイケイゲカ ロジヨウビヨウイン", "name": "整形外科　芦城病院", "prefecture": "石川県", "city": "小松市", "neighborhood": "大文字町", "banchi": "88", "postal_code": "9238552", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ダイモンジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9238581','{"jis": "17203", "kana": "ダイキヨウ カブシキガイシヤ", "name": "大京　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "串町", "banchi": "工業団地1-1", "postal_code": "9238581", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "クシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238578','{"jis": "17203", "kana": "ダイニシヨウジユエン", "name": "第二松寿園", "prefecture": "石川県", "city": "小松市", "neighborhood": "月津町", "banchi": "ヲ95", "postal_code": "9238578", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ツキヅマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238550','{"jis": "17203", "kana": "テイジンカコウシ カブシキガイシヤ", "name": "帝人加工糸　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "今江町", "banchi": "6丁目349", "postal_code": "9238550", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "イマエマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238520','{"jis": "17203", "kana": "トウアデンキコウギヨウ カブシキガイシヤ ピ-アンドデイ-センタ-", "name": "東亜電機工業　株式会社　Ｐ＆Ｄセンター", "prefecture": "石川県", "city": "小松市", "neighborhood": "国府台", "banchi": "5丁目3", "postal_code": "9238520", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "コクフダイ", "alternates": []}');
+INSERT INTO office_data VALUES('9238552','{"jis": "17203", "kana": "トクテイイリヨウホウジンシヤダン カツキカイ ロジヨウクリニツク", "name": "特定医療法人社団　勝木会　芦城クリニック", "prefecture": "石川県", "city": "小松市", "neighborhood": "土居原町", "banchi": "175", "postal_code": "9238552", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": true, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ドイハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238633','{"jis": "17203", "kana": "ニホンデンシンデンワ カブシキガイシヤ コマツシテン", "name": "日本電信電話　株式会社　小松支店", "prefecture": "石川県", "city": "小松市", "neighborhood": "末広町", "banchi": "46", "postal_code": "9238633", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "スエヒロマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238580','{"jis": "17203", "kana": "ブレクスプロダクツ カブシキガイシヤ", "name": "ブレクスプロダクツ　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "里川町", "banchi": "ナ23番地", "postal_code": "9238580", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "サトカワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238528','{"jis": "17203", "kana": "ホクリクジヤスコ シンコマツテン", "name": "北陸ジャスコ　新小松店", "prefecture": "石川県", "city": "小松市", "neighborhood": "平面町", "banchi": "ア69", "postal_code": "9238528", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ヒラオモテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238601','{"jis": "17203", "kana": "ホクリクタイリヨクカガクケンキユウシヨ", "name": "北陸体力科学研究所", "prefecture": "石川県", "city": "小松市", "neighborhood": "八幡", "banchi": "イ13-1", "postal_code": "9238601", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ヤワタ", "alternates": []}');
 INSERT INTO office_data VALUES('9238525','{"jis": "17203", "kana": "ミシマセキユ カブシキガイシヤ", "name": "三島石油　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "問屋町", "banchi": "25", "postal_code": "9238525", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "トンヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238505','{"jis": "17203", "kana": "モリヤス カブシキガイシヤ", "name": "森康　株式会社", "prefecture": "石川県", "city": "小松市", "neighborhood": "光町", "banchi": "89", "postal_code": "9238505", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ヒカリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9238551','{"jis": "17203", "kana": "ヤワタメデイカルセンタ-", "name": "やわたメディカルセンター", "prefecture": "石川県", "city": "小松市", "neighborhood": "八幡", "banchi": "イ12-7", "postal_code": "9238551", "old_code": "923  ", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "イシカワケン", "city_kana": "コマツシ", "neighborhood_kana": "ヤワタ", "alternates": []}');
@@ -132228,16 +132272,16 @@
 INSERT INTO office_data VALUES('9128524','{"jis": "18205", "kana": "オオノカンイサイバンシヨ", "name": "大野簡易裁判所", "prefecture": "福井県", "city": "大野市", "neighborhood": "弥生町", "banchi": "1番11号", "postal_code": "9128524", "old_code": "912  ", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "ヤヨイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9128666','{"jis": "18205", "kana": "オオノシヤクシヨ", "name": "大野市役所", "prefecture": "福井県", "city": "大野市", "neighborhood": "天神町", "banchi": "1-1(大野郵便局私書箱第10号)", "postal_code": "9128666", "old_code": "912  ", "post_office": "大野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "テンジンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9128585','{"jis": "18205", "kana": "オオノシヨツピングセンタ- リブレ", "name": "大野ショッピングセンター　リブレ", "prefecture": "福井県", "city": "大野市", "neighborhood": "月美町", "banchi": "4-8", "postal_code": "9128585", "old_code": "912  ", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "ツキミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9128555','{"jis": "18205", "kana": "オオノゼイムシヨ", "name": "大野税務署", "prefecture": "福井県", "city": "大野市", "neighborhood": "城町", "banchi": "7-28", "postal_code": "9128555", "old_code": "912  ", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9128567','{"jis": "18205", "kana": "キヨウドウクミアイ オオノシヨウギヨウカイハツ シヨツピングモ-ルヴイオ", "name": "協同組合　大野商業開発　ショッピングモールＶｉｏ", "prefecture": "福井県", "city": "大野市", "neighborhood": "鍬掛", "banchi": "17-17-1", "postal_code": "9128567", "old_code": "912  ", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "クワカケ", "alternates": []}');
 INSERT INTO office_data VALUES('9128540','{"jis": "18205", "kana": "テラルエチゼンノウギヨウキヨウドウクミアイ", "name": "テラル越前農業共同組合", "prefecture": "福井県", "city": "大野市", "neighborhood": "中挾", "banchi": "1丁目1301番地", "postal_code": "9128540", "old_code": "912  ", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "ナカバサミ", "alternates": []}');
 INSERT INTO office_data VALUES('9120292','{"jis": "18205", "kana": "オオノシ イズミシシヨ", "name": "大野市　和泉支所", "prefecture": "福井県", "city": "大野市", "neighborhood": "朝日", "banchi": "16-3-4", "postal_code": "9120292", "old_code": "91202", "post_office": "大野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "オオノシ", "neighborhood_kana": "アサヒ", "alternates": []}');
-INSERT INTO office_data VALUES('9118555','{"jis": "18206", "kana": "アボツトジヤパン カブシキガイシヤ カツヤマジギヨウシヨ", "name": "アボットジャパン　株式会社　勝山事業所", "prefecture": "福井県", "city": "勝山市", "neighborhood": "猪野口", "banchi": "37-1-1(勝山郵便局私書箱第4号)", "postal_code": "9118555", "old_code": "911  ", "post_office": "勝山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "イノクチ", "alternates": []}');
 INSERT INTO office_data VALUES('9118501','{"jis": "18206", "kana": "カツヤマシヤクシヨ", "name": "勝山市役所", "prefecture": "福井県", "city": "勝山市", "neighborhood": "元町", "banchi": "1丁目1-1", "postal_code": "9118501", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "モトマチ", "alternates": []}');
+INSERT INTO office_data VALUES('9118555','{"jis": "18206", "kana": "カツヤマフア-マ カブシキガイシヤ", "name": "勝山ファーマ　株式会社", "prefecture": "福井県", "city": "勝山市", "neighborhood": "猪野口", "banchi": "37字2番1号(勝山郵便局私書箱第4号)", "postal_code": "9118555", "old_code": "911  ", "post_office": "勝山", "type": "box", "multiple": false, "new": true, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "イノクチ", "alternates": []}');
 INSERT INTO office_data VALUES('9118585','{"jis": "18206", "kana": "カブシキガイシヤ イツポンギクボホンテン", "name": "株式会社　一本義久保本店", "prefecture": "福井県", "city": "勝山市", "neighborhood": "沢町", "banchi": "1丁目3番1号", "postal_code": "9118585", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "サワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9118510','{"jis": "18206", "kana": "ケイテ-・テクシ-ノ カブシキガイシヤ", "name": "ケイテー・テクシーノ　株式会社", "prefecture": "福井県", "city": "勝山市", "neighborhood": "昭和町", "banchi": "1丁目10-18", "postal_code": "9118510", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "ショウワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9118540','{"jis": "18206", "kana": "フクイケンリツ カツヤマコウトウガツコウ", "name": "福井県立　勝山高等学校", "prefecture": "福井県", "city": "勝山市", "neighborhood": "昭和町", "banchi": "2丁目3-1", "postal_code": "9118540", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "ショウワマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9118601','{"jis": "18206", "kana": "フクイケンリツ キヨウリユウハクブツカン", "name": "福井県立　恐竜博物館", "prefecture": "福井県", "city": "勝山市", "neighborhood": "村岡町寺尾", "banchi": "第51号11番地", "postal_code": "9118601", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "ムロコチョウテラオ", "alternates": []}');
 INSERT INTO office_data VALUES('9118558','{"jis": "18206", "kana": "フクイシヤカイホケンビヨウイン", "name": "福井社会保険病院", "prefecture": "福井県", "city": "勝山市", "neighborhood": "長山町", "banchi": "2丁目6-21", "postal_code": "9118558", "old_code": "911  ", "post_office": "勝山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "ナガヤマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9118531','{"jis": "18206", "kana": "マツブンサンギヨウ カブシキガイシヤ", "name": "松文産業　株式会社", "prefecture": "福井県", "city": "勝山市", "neighborhood": "旭町", "banchi": "1丁目1-56(勝山郵便局私書箱第3号)", "postal_code": "9118531", "old_code": "911  ", "post_office": "勝山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "カツヤマシ", "neighborhood_kana": "アサヒマチ", "alternates": []}');
 INSERT INTO office_data VALUES('9168505','{"jis": "18207", "kana": "アオヤマガンキヨウ カブシキガイシヤ", "name": "青山眼鏡　株式会社", "prefecture": "福井県", "city": "鯖江市", "neighborhood": "神中町", "banchi": "2丁目3-30", "postal_code": "9168505", "old_code": "916  ", "post_office": "鯖江", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "サバエシ", "neighborhood_kana": "カミナカチョウ", "alternates": []}');
@@ -132271,15 +132315,15 @@
 INSERT INTO office_data VALUES('9158511','{"jis": "18209", "kana": "イリヨウホウジン ハヤシビヨウイン", "name": "医療法人　林病院", "prefecture": "福井県", "city": "越前市", "neighborhood": "府中", "banchi": "1丁目5-7", "postal_code": "9158511", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "フチュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158530','{"jis": "18209", "kana": "エチゼンシヤクシヨ", "name": "越前市役所", "prefecture": "福井県", "city": "越前市", "neighborhood": "府中", "banchi": "1丁目13-7", "postal_code": "9158530", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "フチュウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158555','{"jis": "18209", "kana": "オリオンデンキ カブシキガイシヤ", "name": "オリオン電機　株式会社", "prefecture": "福井県", "city": "越前市", "neighborhood": "家久町", "banchi": "41-1", "postal_code": "9158555", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "イエヒサチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158520','{"jis": "18209", "kana": "カブシキガイシヤ アイシンフクイ", "name": "株式会社　アイシン福井", "prefecture": "福井県", "city": "越前市", "neighborhood": "池ノ上町", "banchi": "38", "postal_code": "9158520", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "イケノカミチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158666','{"jis": "18209", "kana": "カブシキガイシヤ タケフセイメン", "name": "株式会社　武生製麺", "prefecture": "福井県", "city": "越前市", "neighborhood": "真柄町", "banchi": "7-37", "postal_code": "9158666", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "マカラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158501','{"jis": "18209", "kana": "カブシキガイシヤ フジヤシヨクヒン", "name": "株式会社　ふじや食品", "prefecture": "福井県", "city": "越前市", "neighborhood": "矢船町", "banchi": "1丁目7-1", "postal_code": "9158501", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "ヤフネチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158585','{"jis": "18209", "kana": "キハラケンセツ カブシキガイシヤ", "name": "木原建設　株式会社", "prefecture": "福井県", "city": "越前市", "neighborhood": "大虫町", "banchi": "7-2", "postal_code": "9158585", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "オオムシチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('9158577','{"jis": "18209", "kana": "キヨ-セ- カブシキガイシヤ", "name": "キョーセー　株式会社", "prefecture": "福井県", "city": "越前市", "neighborhood": "妙法寺町", "banchi": "29号2", "postal_code": "9158577", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "ミョウホウジチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('9158577','{"jis": "18209", "kana": "キヨ-セ- カブシキガイシヤ", "name": "キョーセー　株式会社", "prefecture": "福井県", "city": "越前市", "neighborhood": "妙法寺町", "banchi": "29号2", "postal_code": "9158577", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "ミョウホウジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158515','{"jis": "18209", "kana": "シンエツカガクコウギヨウ カブシキガイシヤ タケフコウジヨウ", "name": "信越化学工業　株式会社　武生工場", "prefecture": "福井県", "city": "越前市", "neighborhood": "北府", "banchi": "2-1-5", "postal_code": "9158515", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "キタゴ", "alternates": []}');
 INSERT INTO office_data VALUES('9158586','{"jis": "18209", "kana": "ジンアイダイガク", "name": "仁愛大学", "prefecture": "福井県", "city": "越前市", "neighborhood": "大手町", "banchi": "3-1-1", "postal_code": "9158586", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "オオデチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158533','{"jis": "18209", "kana": "タケフゼイムシヨ", "name": "武生税務署", "prefecture": "福井県", "city": "越前市", "neighborhood": "中央", "banchi": "1丁目6-12", "postal_code": "9158533", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158588','{"jis": "18209", "kana": "タンナンケ-ブルテレビ カブシキガイシヤ", "name": "丹南ケーブルテレビ　株式会社", "prefecture": "福井県", "city": "越前市", "neighborhood": "塚町", "banchi": "101番地", "postal_code": "9158588", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "ツカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158510','{"jis": "18209", "kana": "フクイケン ナンエツケンゼイジムシヨ", "name": "福井県　南越県税事務所", "prefecture": "福井県", "city": "越前市", "neighborhood": "上太田町", "banchi": "41-5", "postal_code": "9158510", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "カミオオダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('9158524','{"jis": "18209", "kana": "フクイチホウサイバンシヨタケフシブ、フクイカテイサイバンシヨタケフシブ、タケフカンイサイバンシヨ", "name": "福井地方裁判所武生支部、福井家庭裁判所武生支部、武生簡易裁判所", "prefecture": "福井県", "city": "越前市", "neighborhood": "日野美", "banchi": "二丁目6番地", "postal_code": "9158524", "old_code": "915  ", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "ヒノミ", "alternates": []}');
 INSERT INTO office_data VALUES('9150292','{"jis": "18209", "kana": "エチゼンシ イマダテソウゴウシシヨ", "name": "越前市　今立総合支所", "prefecture": "福井県", "city": "越前市", "neighborhood": "粟田部町", "banchi": "11-35", "postal_code": "9150292", "old_code": "91502", "post_office": "武生", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクイケン", "city_kana": "エチゼンシ", "neighborhood_kana": "アワタベチョウ", "alternates": []}');
@@ -132536,15 +132580,15 @@
 INSERT INTO office_data VALUES('3808648','{"jis": "20201", "kana": "ダイイチセイメイホケン カブシキガイシヤ ナガノシシヤ", "name": "第一生命保険　株式会社　長野支社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字中御所", "banchi": "219-1(長野中央郵便局私書箱第38号)", "postal_code": "3808648", "old_code": "380  ", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808566','{"jis": "20201", "kana": "ダイイチホウキシユツパン カブシキガイシヤ", "name": "第一法規出版　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字中御所", "banchi": "岡田町176", "postal_code": "3808566", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808505','{"jis": "20201", "kana": "ダイワハウスコウギヨウ カブシキガイシヤ ナガノシテン", "name": "大和ハウス工業　株式会社　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "", "banchi": "荒屋1180-1", "postal_code": "3808505", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808575','{"jis": "20201", "kana": "チユウブシンリンカンリキヨク", "name": "中部森林管理局", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字栗田", "banchi": "715-5", "postal_code": "3808575", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808601','{"jis": "20201", "kana": "テルウエルヒガシニツポン カブシキカイシヤ ナガノシテン", "name": "テルウェル東日本　株式会社　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "新田町", "banchi": "1137-5NTT新田町ビル", "postal_code": "3808601", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "シンデンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3808508','{"jis": "20201", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキガイシヤ ナガノシテン", "name": "東京海上日動火災保険　株式会社　長野支店", "prefecture": "長野県", "city": "長野市", "neighborhood": "", "banchi": "南県町1081長野東京海上日動ビル", "postal_code": "3808508", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808688','{"jis": "20201", "kana": "トウキヨウホウレイシユツパン カブシキガイシヤ", "name": "東京法令出版　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字鶴賀", "banchi": "南千歳町1005(長野中央郵便局私書箱第17号)", "postal_code": "3808688", "old_code": "380  ", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('3808550','{"jis": "20201", "kana": "ナガノアサヒホウソウ カブシキガイシヤ", "name": "長野朝日放送　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "七瀬", "banchi": "4-5", "postal_code": "3808550", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ナナセ", "alternates": []}');
+INSERT INTO office_data VALUES('3808550','{"jis": "20201", "kana": "ナガノアサヒホウソウ カブシキガイシヤ", "name": "長野朝日放送　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "七瀬", "banchi": "4-5", "postal_code": "3808550", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ナナセ", "alternates": []}');
 INSERT INTO office_data VALUES('3808586','{"jis": "20201", "kana": "ナガノケン シチヨウソンシヨクインキヨウサイクミアイ", "name": "長野県　市町村職員共済組合", "prefecture": "長野県", "city": "長野市", "neighborhood": "権堂町", "banchi": "2201番地", "postal_code": "3808586", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ゴンドウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('3808535','{"jis": "20201", "kana": "ナガノケン シヤカイホケンシンリヨウホウシユウシハライキキン", "name": "長野県　社会保険診療報酬支払基金", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字鶴賀", "banchi": "1457番地44", "postal_code": "3808535", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808668','{"jis": "20201", "kana": "ナガノケン シンヨウクミアイ", "name": "長野県　信用組合", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長野", "banchi": "新田町1103-1(長野中央郵便局私書箱第70号)", "postal_code": "3808668", "old_code": "380  ", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808611','{"jis": "20201", "kana": "ナガノケン ロウドウキンコ", "name": "長野県　労働金庫", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長野", "banchi": "県町523(長野中央郵便局私書箱第90号)", "postal_code": "3808611", "old_code": "380  ", "post_office": "長野中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808510','{"jis": "20201", "kana": "ナガノケンケイサツホンブ", "name": "長野県警察本部", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字南長野", "banchi": "字巾下692-2", "postal_code": "3808510", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808551','{"jis": "20201", "kana": "ナガノケンシユルイハンバイ カブシキガイシヤ", "name": "長野県酒類販売　株式会社", "prefecture": "長野県", "city": "長野市", "neighborhood": "大字稲葉", "banchi": "日詰1414", "postal_code": "3808551", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('3808515','{"jis": "20201", "kana": "ナガノケンナガノコウトウガツコウ", "name": "長野県長野高等学校", "prefecture": "長野県", "city": "長野市", "neighborhood": "上松", "banchi": "1丁目16-12", "postal_code": "3808515", "old_code": "380  ", "post_office": "長野中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ナガノケン", "city_kana": "ナガノシ", "neighborhood_kana": "ウエマツ", "alternates": []}');
@@ -136356,15 +136400,15 @@
 INSERT INTO office_data VALUES('6008588','{"jis": "26106", "kana": "キヨウトシシモギヨウクヤクシヨ", "name": "京都市下京区役所", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "西洞院通塩小路上る", "banchi": "東塩小路町608-8", "postal_code": "6008588", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008565','{"jis": "26106", "kana": "キヨウトシヨウコウカイギシヨ", "name": "京都商工会議所", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通室町東入", "banchi": "函谷鉾町78京都経済センター7階", "postal_code": "6008565", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008787','{"jis": "26106", "kana": "キヨウトチイキセンタ-", "name": "京都地域センター", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "東塩小路町", "banchi": "843-12(京都中央郵便局内)", "postal_code": "6008787", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "キョウトフ", "city_kana": "キョウトシシモギョウク", "neighborhood_kana": "ヒガシシオコウジチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6008665','{"jis": "26106", "kana": "キヨウトチユウオウシンヨウキンコ", "name": "京都中央信用金庫", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通室町東入", "banchi": "函谷鉾町91(京都中央郵便局私書箱第86号)", "postal_code": "6008665", "old_code": "600  ", "post_office": "京都中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008585','{"jis": "26106", "kana": "コウエキザイダンホウジン ニホンカンジノウリヨクケンテイキヨウカイ", "name": "公益財団法人　日本漢字能力検定協会", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "烏丸通松原下る", "banchi": "五条烏丸町398番地", "postal_code": "6008585", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008505','{"jis": "26106", "kana": "シンシユウオオタニハ (ヒガシホンガンジ) シユウムシヨ", "name": "真宗大谷派　（東本願寺）　宗務所", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "烏丸通七条上る", "banchi": "常葉町754", "postal_code": "6008505", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008501','{"jis": "26106", "kana": "ジヨウドシンシユウホンガンジハシユウムシヨ", "name": "浄土真宗本願寺派宗務所", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "堀川通花屋町下る", "banchi": "本願寺門前町", "postal_code": "6008501", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('6008522','{"jis": "26106", "kana": "ゼンコクケンコウホケンキヨウカイ キヨウトシブ", "name": "全国健康保険協会　京都支部", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通麩屋町西入", "banchi": "立売東町28-2大和証券京都ビル2階", "postal_code": "6008522", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('6008522','{"jis": "26106", "kana": "ゼンコクケンコウホケンキヨウカイ キヨウトシブ", "name": "全国健康保険協会　京都支部", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通麩屋町西入", "banchi": "立売東町28-2大和証券京都ビル2階", "postal_code": "6008522", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008688','{"jis": "26106", "kana": "タカラホ-ルデイングス カブシキガイシヤ", "name": "宝ホールディングス　株式会社", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通烏丸東入", "banchi": "長刀鉾町20番地", "postal_code": "6008688", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008686','{"jis": "26106", "kana": "タキイシユビヨウ カブシキガイシヤ", "name": "タキイ種苗　株式会社", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "梅小路通猪熊東入", "banchi": "南夷町180(京都中央郵便局私書箱第7号)", "postal_code": "6008686", "old_code": "600  ", "post_office": "京都中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008570','{"jis": "26106", "kana": "トウキヨウカイジヨウニチドウカサイホケン カブシキカイシヤ", "name": "東京海上日動火災保険　株式会社", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "四条通麩屋町西入", "banchi": "立売東町22", "postal_code": "6008570", "old_code": "600  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6008652','{"jis": "26106", "kana": "カブシキガイシヤ キヨウトギンコウ", "name": "株式会社　京都銀行", "prefecture": "京都府", "city": "京都市下京区", "neighborhood": "烏丸通松原上る", "banchi": "薬師前町700(京都中央郵便局私書箱第80号)", "postal_code": "6008652", "old_code": "60091", "post_office": "京都中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('6018601','{"jis": "26107", "kana": "イオンモ-ルキヨウトカツラガワ", "name": "イオンモール京都桂川", "prefecture": "京都府", "city": "京都市南区", "neighborhood": "久世高田町", "banchi": "376番1号", "postal_code": "6018601", "old_code": "601  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "キョウトフ", "city_kana": "キョウトシミナミク", "neighborhood_kana": "クゼタカダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6018542','{"jis": "26107", "kana": "エヌテイテイフアイナンス カブシキガイシヤ ニシニホンミヤコリヨウキンセンタ-", "name": "ＮＴＴファイナンス　株式会社　西日本みやこ料金センター", "prefecture": "京都府", "city": "京都市南区", "neighborhood": "西九条菅田町", "banchi": "19-1", "postal_code": "6018542", "old_code": "601  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "キョウトフ", "city_kana": "キョウトシミナミク", "neighborhood_kana": "ニシクジョウスガタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6018560','{"jis": "26107", "kana": "カブシキカイシヤ キンデン キヨウトシテン", "name": "株式会社　きんでん　京都支店", "prefecture": "京都府", "city": "京都市南区", "neighborhood": "西九条西柳ノ内町", "banchi": "8番地", "postal_code": "6018560", "old_code": "601  ", "post_office": "京都中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "キョウトフ", "city_kana": "キョウトシミナミク", "neighborhood_kana": "ニシクジョウニシヤナギノウチチョウ", "alternates": []}');
@@ -137146,15 +137190,15 @@
 INSERT INTO office_data VALUES('5708787','{"jis": "27209", "kana": "オオサカコクサイチユウガツコウコウトウガツコウ", "name": "大阪国際中学校高等学校", "prefecture": "大阪府", "city": "守口市", "neighborhood": "松下町", "banchi": "1番28号", "postal_code": "5708787", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "マツシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708539','{"jis": "27209", "kana": "オクムラキカイ (カ", "name": "奥村機械　（株）", "prefecture": "大阪府", "city": "守口市", "neighborhood": "佐太中町", "banchi": "2丁目5-3", "postal_code": "5708539", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "サタナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5708558','{"jis": "27209", "kana": "カブシキガイシヤ ケイハンヒヤツカテン", "name": "株式会社　京阪百貨店", "prefecture": "大阪府", "city": "守口市", "neighborhood": "河原町", "banchi": "8-3", "postal_code": "5708558", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "カワハラチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708506','{"jis": "27209", "kana": "カンサイイカダイガク", "name": "関西医科大学", "prefecture": "大阪府", "city": "守口市", "neighborhood": "文園町", "banchi": "10-15", "postal_code": "5708506", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "フミゾノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708507','{"jis": "27209", "kana": "カンサイイカダイガクソウゴウイリヨウセンタ-", "name": "関西医科大学総合医療センター", "prefecture": "大阪府", "city": "守口市", "neighborhood": "文園町", "banchi": "10-15", "postal_code": "5708507", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "フミゾノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708555','{"jis": "27209", "kana": "ガツコウホウジン オオサカコクサイガクエン・オオサカコクサイダイガク・オオサカコクサイダイガクタンキダイガクブ", "name": "学校法人　大阪国際学園・大阪国際大学・大阪国際大学短期大学部", "prefecture": "大阪府", "city": "守口市", "neighborhood": "藤田町", "banchi": "6丁目21番57号", "postal_code": "5708555", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "トウダチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708634','{"jis": "27209", "kana": "サンヨウデンキボウエキ カブシキガイシヤ", "name": "三洋電機貿易　株式会社", "prefecture": "大阪府", "city": "守口市", "neighborhood": "日吉町", "banchi": "2丁目5-15(守口郵便局私書箱第18号)", "postal_code": "5708634", "old_code": "570  ", "post_office": "守口", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヒヨシチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('5708511','{"jis": "27209", "kana": "パナソニツクエナジ- カブシキガイシヤ", "name": "パナソニックエナジー　株式会社", "prefecture": "大阪府", "city": "守口市", "neighborhood": "松下町", "banchi": "1番1号", "postal_code": "5708511", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "マツシタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('5708511','{"jis": "27209", "kana": "パナソニツクエナジ- カブシキガイシヤ", "name": "パナソニックエナジー　株式会社", "prefecture": "大阪府", "city": "守口市", "neighborhood": "松下町", "banchi": "1番1号", "postal_code": "5708511", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "マツシタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708540','{"jis": "27209", "kana": "マツシタデンキ ケンコウホケンクミアイ・マツシタキネンビヨウイン・マツシタケンコウカンリセンタ-", "name": "松下電器　健康保険組合・松下記念病院・松下健康管理センター", "prefecture": "大阪府", "city": "守口市", "neighborhood": "外島町", "banchi": "5-55", "postal_code": "5708540", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ソトジマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5708501','{"jis": "27209", "kana": "マツシタデンキサンギヨウ カブシキガイシヤ ギジユツソウムセンタ-", "name": "松下電器産業　（株）　技術総務センター", "prefecture": "大阪府", "city": "守口市", "neighborhood": "八雲中町", "banchi": "3丁目1-1", "postal_code": "5708501", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ヤグモナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5708666','{"jis": "27209", "kana": "モリグチシヤクシヨ", "name": "守口市役所", "prefecture": "大阪府", "city": "守口市", "neighborhood": "京阪本通", "banchi": "2丁目5-5(守口郵便局私書箱第1号)", "postal_code": "5708666", "old_code": "570  ", "post_office": "守口", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "ケイハンホンドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('5708585','{"jis": "27209", "kana": "ヤマオカキンゾクコウギヨウ カブシキガイシヤ", "name": "山岡金属工業　株式会社", "prefecture": "大阪府", "city": "守口市", "neighborhood": "東郷通", "banchi": "2丁目7番30号", "postal_code": "5708585", "old_code": "570  ", "post_office": "守口", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "モリグチシ", "neighborhood_kana": "トウゴウドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('5731040','{"jis": "27210", "kana": "(カブ) ヒラカタジドウシヤキヨウシユウジヨ", "name": "（株）　枚方自動車教習所", "prefecture": "大阪府", "city": "枚方市", "neighborhood": "招提東町", "banchi": "1丁目1番1号", "postal_code": "5731040", "old_code": "573  ", "post_office": "枚方北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヒラカタシ", "neighborhood_kana": "ショウダイヒガシマチ", "alternates": []}');
 INSERT INTO office_data VALUES('5738588','{"jis": "27210", "kana": "オオサカホウムキヨク ヒラカタシユツチヨウシヨ", "name": "大阪法務局　枚方出張所", "prefecture": "大阪府", "city": "枚方市", "neighborhood": "大垣内町", "banchi": "2丁目4-6", "postal_code": "5738588", "old_code": "573  ", "post_office": "枚方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヒラカタシ", "neighborhood_kana": "オオガイトチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5738510','{"jis": "27210", "kana": "カブシキガイシヤ カンサイパド", "name": "株式会社　関西ぱど", "prefecture": "大阪府", "city": "枚方市", "neighborhood": "三矢町", "banchi": "5-18メゾン枚方ビル1F", "postal_code": "5738510", "old_code": "573  ", "post_office": "枚方", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オオサカフ", "city_kana": "ヒラカタシ", "neighborhood_kana": "ミツヤチョウ", "alternates": []}');
@@ -137633,15 +137677,15 @@
 INSERT INTO office_data VALUES('6638558','{"jis": "28204", "kana": "ガツコウホウジン ムコガワガクイン", "name": "学校法人　武庫川学院", "prefecture": "兵庫県", "city": "西宮市", "neighborhood": "池開町", "banchi": "6-46", "postal_code": "6638558", "old_code": "663  ", "post_office": "西宮東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ニシノミヤシ", "neighborhood_kana": "イケビラキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6638545','{"jis": "28204", "kana": "キヨクトウカイハツコウギヨウ カブシキガイシヤ", "name": "極東開発工業　株式会社", "prefecture": "兵庫県", "city": "西宮市", "neighborhood": "甲子園口", "banchi": "6丁目1-45", "postal_code": "6638545", "old_code": "663  ", "post_office": "西宮東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ニシノミヤシ", "neighborhood_kana": "コウシエングチ", "alternates": []}');
 INSERT INTO office_data VALUES('6638567','{"jis": "28204", "kana": "ニツポンネンキンキコウ ニシノミヤネンキンジムシヨ", "name": "日本年金機構　西宮年金事務所", "prefecture": "兵庫県", "city": "西宮市", "neighborhood": "津門大塚町", "banchi": "8-26", "postal_code": "6638567", "old_code": "663  ", "post_office": "西宮東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ニシノミヤシ", "neighborhood_kana": "ツトオオツカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6638585','{"jis": "28204", "kana": "ヌノカメ カブシキガイシヤ", "name": "布亀　株式会社", "prefecture": "兵庫県", "city": "西宮市", "neighborhood": "今津二葉町", "banchi": "2-6", "postal_code": "6638585", "old_code": "663  ", "post_office": "西宮東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "ニシノミヤシ", "neighborhood_kana": "イマヅフタバチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6568686','{"jis": "28205", "kana": "スモトシヤクシヨ", "name": "洲本市役所", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "本町", "banchi": "3丁目4-10(洲本郵便局私書箱第6号)", "postal_code": "6568686", "old_code": "656  ", "post_office": "洲本", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6568656','{"jis": "28205", "kana": "スモトゼイムシヨ", "name": "洲本税務署", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "山手", "banchi": "1-1-15", "postal_code": "6568656", "old_code": "656  ", "post_office": "洲本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "ヤマテ", "alternates": []}');
 INSERT INTO office_data VALUES('6568666','{"jis": "28205", "kana": "ダンヨウシンヨウクミアイ", "name": "淡陽信用組合", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "栄町", "banchi": "1丁目3-17(洲本郵便局私書箱第14号)", "postal_code": "6568666", "old_code": "656  ", "post_office": "洲本", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "サカエマチ", "alternates": []}');
-INSERT INTO office_data VALUES('6568555','{"jis": "28205", "kana": "パナソニツクエナジ- カブシキガイシヤ", "name": "パナソニックエナジー　株式会社", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "上内膳", "banchi": "222-1", "postal_code": "6568555", "old_code": "656  ", "post_office": "洲本", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "カミナイゼン", "alternates": []}');
+INSERT INTO office_data VALUES('6568555','{"jis": "28205", "kana": "パナソニツクエナジ- カブシキガイシヤ", "name": "パナソニックエナジー　株式会社", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "上内膳", "banchi": "222-1", "postal_code": "6568555", "old_code": "656  ", "post_office": "洲本", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "カミナイゼン", "alternates": []}');
 INSERT INTO office_data VALUES('6561395','{"jis": "28205", "kana": "スモトシヤクシヨ ゴシキチヨウシヤ", "name": "洲本市役所　五色庁舎", "prefecture": "兵庫県", "city": "洲本市", "neighborhood": "五色町都志", "banchi": "203", "postal_code": "6561395", "old_code": "65613", "post_office": "五色", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "スモトシ", "neighborhood_kana": "ゴシキチョウツシ", "alternates": []}');
 INSERT INTO office_data VALUES('6598511','{"jis": "28206", "kana": "ガツコウホウジン アシヤガクエン", "name": "学校法人　芦屋学園", "prefecture": "兵庫県", "city": "芦屋市", "neighborhood": "六麓荘町", "banchi": "13-22", "postal_code": "6598511", "old_code": "569  ", "post_office": "芦屋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アシヤシ", "neighborhood_kana": "ロクロクソウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6598501','{"jis": "28206", "kana": "アシヤシヤクシヨ", "name": "芦屋市役所", "prefecture": "兵庫県", "city": "芦屋市", "neighborhood": "精道町", "banchi": "7-6", "postal_code": "6598501", "old_code": "659  ", "post_office": "芦屋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アシヤシ", "neighborhood_kana": "セイドウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6598503','{"jis": "28206", "kana": "アシヤゼイムシヨ", "name": "芦屋税務署", "prefecture": "兵庫県", "city": "芦屋市", "neighborhood": "公光町", "banchi": "6-2", "postal_code": "6598503", "old_code": "659  ", "post_office": "芦屋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アシヤシ", "neighborhood_kana": "キンミツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6598502','{"jis": "28206", "kana": "シリツ アシヤビヨウイン", "name": "市立　芦屋病院", "prefecture": "兵庫県", "city": "芦屋市", "neighborhood": "朝日ケ丘町", "banchi": "39-1", "postal_code": "6598502", "old_code": "659  ", "post_office": "芦屋", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アシヤシ", "neighborhood_kana": "アサヒガオカチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('5398794','{"jis": "28207", "kana": "オオサカチヨキンジムセンタ-", "name": "大阪貯金事務センター", "prefecture": "兵庫県", "city": "伊丹市", "neighborhood": "北河原", "banchi": "1-2-1", "postal_code": "5398794", "old_code": "53999", "post_office": "新大阪", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "イタミシ", "neighborhood_kana": "キタガワラ", "alternates": []}');
 INSERT INTO office_data VALUES('6648545','{"jis": "28207", "kana": "イタミカンイサイバンシヨ", "name": "伊丹簡易裁判所", "prefecture": "兵庫県", "city": "伊丹市", "neighborhood": "千僧", "banchi": "1丁目47-1", "postal_code": "6648545", "old_code": "664  ", "post_office": "伊丹", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "イタミシ", "neighborhood_kana": "センゾ", "alternates": []}');
@@ -137828,15 +137872,15 @@
 INSERT INTO office_data VALUES('6792282','{"jis": "28443", "kana": "チユウシヨウキギヨウダイガツコウカンサイコウ", "name": "中小企業大学校関西校", "prefecture": "兵庫県", "city": "神崎郡福崎町", "neighborhood": "高岡", "banchi": "1929", "postal_code": "6792282", "old_code": "67922", "post_office": "福崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "カンザキグンフクサキチョウ", "neighborhood_kana": "タカオカ", "alternates": []}');
 INSERT INTO office_data VALUES('6792283','{"jis": "28443", "kana": "トツパンインサツ カブシキガイシヤ フクサキコウジヨウ", "name": "凸版印刷　株式会社　福崎工場", "prefecture": "兵庫県", "city": "神崎郡福崎町", "neighborhood": "高橋", "banchi": "290-29", "postal_code": "6792283", "old_code": "67922", "post_office": "福崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "カンザキグンフクサキチョウ", "neighborhood_kana": "タカハシ", "alternates": []}');
 INSERT INTO office_data VALUES('6792280','{"jis": "28443", "kana": "フクサキチヨウヤクバ", "name": "福崎町役場", "prefecture": "兵庫県", "city": "神崎郡福崎町", "neighborhood": "南田原", "banchi": "3116-1(福崎郵便局私書箱第4号)", "postal_code": "6792280", "old_code": "67922", "post_office": "福崎", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "カンザキグンフクサキチョウ", "neighborhood_kana": "ミナミタワラ", "alternates": []}');
 INSERT INTO office_data VALUES('6792288','{"jis": "28443", "kana": "フクシンデンキ カブシキガイシヤ", "name": "福伸電機　株式会社", "prefecture": "兵庫県", "city": "神崎郡福崎町", "neighborhood": "福田", "banchi": "447-1", "postal_code": "6792288", "old_code": "67922", "post_office": "福崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "カンザキグンフクサキチョウ", "neighborhood_kana": "フクダ", "alternates": []}');
 INSERT INTO office_data VALUES('6792493','{"jis": "28446", "kana": "コウリツカンザキソウゴウビヨウイン", "name": "公立神崎総合病院", "prefecture": "兵庫県", "city": "神崎郡神河町", "neighborhood": "粟賀町", "banchi": "385", "postal_code": "6792493", "old_code": "67924", "post_office": "神崎", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "カンザキグンカミカワチョウ", "neighborhood_kana": "アワガマチ", "alternates": []}');
 INSERT INTO office_data VALUES('6711593','{"jis": "28464", "kana": "カブシキガイシヤ ウカイヤ", "name": "株式会社　うかいや", "prefecture": "兵庫県", "city": "揖保郡太子町", "neighborhood": "東出", "banchi": "262-1(太子郵便局私書箱第2号)", "postal_code": "6711593", "old_code": "67115", "post_office": "太子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "イボグンタイシチョウ", "neighborhood_kana": "トウデ", "alternates": []}');
 INSERT INTO office_data VALUES('6711595','{"jis": "28464", "kana": "カブシキガイシヤ トウシバヒメジコウジヨウタイシブンコウジヨウ", "name": "株式会社　東芝姫路工場太子分工場", "prefecture": "兵庫県", "city": "揖保郡太子町", "neighborhood": "鵤", "banchi": "300", "postal_code": "6711595", "old_code": "67115", "post_office": "太子", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "イボグンタイシチョウ", "neighborhood_kana": "イカルガ", "alternates": []}');
-INSERT INTO office_data VALUES('6711592','{"jis": "28464", "kana": "タイシチヨウヤクバ", "name": "太子町役場", "prefecture": "兵庫県", "city": "揖保郡太子町", "neighborhood": "鵤", "banchi": "1369-1(太子郵便局私書箱第6号)", "postal_code": "6711592", "old_code": "67115", "post_office": "太子", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "イボグンタイシチョウ", "neighborhood_kana": "イカルガ", "alternates": []}');
+INSERT INTO office_data VALUES('6711592','{"jis": "28464", "kana": "ヒヨウゴケンイボグンタイシチヨウヤクバ", "name": "兵庫県揖保郡太子町役場", "prefecture": "兵庫県", "city": "揖保郡太子町", "neighborhood": "鵤", "banchi": "280番地1", "postal_code": "6711592", "old_code": "67115", "post_office": "太子", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヒョウゴケン", "city_kana": "イボグンタイシチョウ", "neighborhood_kana": "イカルガ", "alternates": []}');
 INSERT INTO office_data VALUES('6781292','{"jis": "28481", "kana": "カミゴオリチヨウヤクバ", "name": "上郡町役場", "prefecture": "兵庫県", "city": "赤穂郡上郡町", "neighborhood": "大持", "banchi": "278", "postal_code": "6781292", "old_code": "67812", "post_office": "上郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アコウグンカミゴオリチョウ", "neighborhood_kana": "ダイモチ", "alternates": []}');
 INSERT INTO office_data VALUES('6781295','{"jis": "28481", "kana": "ヒヨウゴケン ニシハリマケンミンキヨク カミゴオリケンゼイジムシヨ", "name": "兵庫県　西播磨県民局　上郡県税事務所", "prefecture": "兵庫県", "city": "赤穂郡上郡町", "neighborhood": "光都", "banchi": "2丁目25", "postal_code": "6781295", "old_code": "67812", "post_office": "上郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アコウグンカミゴオリチョウ", "neighborhood_kana": "コウト", "alternates": []}');
 INSERT INTO office_data VALUES('6781297','{"jis": "28481", "kana": "ヒヨウゴケンリツダイガク リガクブ", "name": "兵庫県立大学　理学部", "prefecture": "兵庫県", "city": "赤穂郡上郡町", "neighborhood": "光都", "banchi": "3丁目2-1", "postal_code": "6781297", "old_code": "67812", "post_office": "上郡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "アコウグンカミゴオリチョウ", "neighborhood_kana": "コウト", "alternates": []}');
 INSERT INTO office_data VALUES('6795192','{"jis": "28501", "kana": "サヨウチヨウヤクバ ミカヅキシシヨ", "name": "佐用町役場　三日月支所", "prefecture": "兵庫県", "city": "佐用郡佐用町", "neighborhood": "三日月", "banchi": "1110-1", "postal_code": "6795192", "old_code": "67951", "post_office": "三日月", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "サヨウグンサヨウチョウ", "neighborhood_kana": "ミカヅキ", "alternates": []}');
 INSERT INTO office_data VALUES('6795198','{"jis": "28501", "kana": "ザイダンホウジン コウキドヒカリカガクケンキユウセンタ-", "name": "財団法人　高輝度光科学研究センター", "prefecture": "兵庫県", "city": "佐用郡佐用町", "neighborhood": "光都", "banchi": "1丁目1番1号", "postal_code": "6795198", "old_code": "67951", "post_office": "三日月", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "サヨウグンサヨウチョウ", "neighborhood_kana": "コウト", "alternates": []}');
 INSERT INTO office_data VALUES('6795292','{"jis": "28501", "kana": "サヨウチヨウヤクバ ナンコウシシヨ", "name": "佐用町役場　南光支所", "prefecture": "兵庫県", "city": "佐用郡佐用町", "neighborhood": "下徳久", "banchi": "1004-1", "postal_code": "6795292", "old_code": "67952", "post_office": "佐用", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "サヨウグンサヨウチョウ", "neighborhood_kana": "シモトクサ", "alternates": []}');
 INSERT INTO office_data VALUES('6795383','{"jis": "28501", "kana": "イリヨウホウジン セイイカイ サヨウチユウオウビヨウイン", "name": "医療法人　聖医会　佐用中央病院", "prefecture": "兵庫県", "city": "佐用郡佐用町", "neighborhood": "佐用", "banchi": "3529-3", "postal_code": "6795383", "old_code": "67953", "post_office": "佐用", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヒョウゴケン", "city_kana": "サヨウグンサヨウチョウ", "neighborhood_kana": "サヨウ", "alternates": []}');
@@ -138352,18 +138396,18 @@
 INSERT INTO office_data VALUES('6988650','{"jis": "32204", "kana": "マスダシヤクシヨ", "name": "益田市役所", "prefecture": "島根県", "city": "益田市", "neighborhood": "常盤町", "banchi": "1-1(益田郵便局私書箱第4号)", "postal_code": "6988650", "old_code": "698  ", "post_office": "益田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "トキワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6988501','{"jis": "32204", "kana": "マスダセキジユウジビヨウイン", "name": "益田赤十字病院", "prefecture": "島根県", "city": "益田市", "neighborhood": "乙吉町", "banchi": "イ103-1", "postal_code": "6988501", "old_code": "698  ", "post_office": "益田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "オトヨシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6980292','{"jis": "32204", "kana": "マスダシヤクシヨミトソウゴウシシヨ", "name": "益田市役所美都総合支所", "prefecture": "島根県", "city": "益田市", "neighborhood": "美都町都茂", "banchi": "1803-1", "postal_code": "6980292", "old_code": "69802", "post_office": "美都", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "マスダシ", "neighborhood_kana": "ミトチョウツモ", "alternates": []}');
 INSERT INTO office_data VALUES('6948501','{"jis": "32205", "kana": "イワミオオダゼイムシヨ", "name": "石見大田税務署", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "イ289-2", "postal_code": "6948501", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
 INSERT INTO office_data VALUES('6948502','{"jis": "32205", "kana": "オオダシヤクシヨ", "name": "大田市役所", "prefecture": "島根県", "city": "大田市", "neighborhood": "大田町大田", "banchi": "ロ1111番地", "postal_code": "6948502", "old_code": "694  ", "post_office": "石見大田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "オオダチョウオオダ", "alternates": []}');
 INSERT INTO office_data VALUES('6992598','{"jis": "32205", "kana": "オオダシヤクシヨ ユノツシシヨ", "name": "大田市役所　温泉津支所", "prefecture": "島根県", "city": "大田市", "neighborhood": "温泉津町小浜", "banchi": "イ486", "postal_code": "6992598", "old_code": "69925", "post_office": "温泉津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "オオダシ", "neighborhood_kana": "ユノツチョウコハマ", "alternates": []}');
 INSERT INTO office_data VALUES('6928506','{"jis": "32206", "kana": "カブシキガイシヤ サンレイフ-ズヤスギエイギヨウシヨ", "name": "（株）　さんれいフーズ安来営業所", "prefecture": "島根県", "city": "安来市", "neighborhood": "亀島町", "banchi": "12-3", "postal_code": "6928506", "old_code": "692  ", "post_office": "安来", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "カメシマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('6928606','{"jis": "32206", "kana": "カブシキガイシヤ ヒタチキンゾクヤスギセイサクシヨ", "name": "株式会社　日立金属安来製作所", "prefecture": "島根県", "city": "安来市", "neighborhood": "飯島町", "banchi": "1240番地5(安来郵便局私書箱第6号)", "postal_code": "6928606", "old_code": "692  ", "post_office": "安来", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "ハシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6928510','{"jis": "32206", "kana": "カブシキガイシヤ フ-ズマ-ケツトホツク", "name": "株式会社　フーズマーケットホック", "prefecture": "島根県", "city": "安来市", "neighborhood": "赤江町", "banchi": "1448-1", "postal_code": "6928510", "old_code": "692  ", "post_office": "安来", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "アカエチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6928601','{"jis": "32206", "kana": "カブシキガイシヤ プロテリアル ヤスギコウジヨウ", "name": "株式会社　プロテリアル　安来工場", "prefecture": "島根県", "city": "安来市", "neighborhood": "安来町", "banchi": "2107-2(安来郵便局私書箱第1号)", "postal_code": "6928601", "old_code": "692  ", "post_office": "安来", "type": "box", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "ヤスギチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('6928606','{"jis": "32206", "kana": "カブシキガイシヤ プロテリアルヤスギセイサクシヨ", "name": "株式会社　プロテリアル安来製作所", "prefecture": "島根県", "city": "安来市", "neighborhood": "飯島町", "banchi": "1240番地2(安来郵便局私書箱第6号)", "postal_code": "6928606", "old_code": "692  ", "post_office": "安来", "type": "box", "multiple": false, "new": true, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "ハシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6928550','{"jis": "32206", "kana": "タカバヤシシヨウジ カブシキカイシヤ", "name": "高林商事　株式会社", "prefecture": "島根県", "city": "安来市", "neighborhood": "恵乃島町", "banchi": "113-16", "postal_code": "6928550", "old_code": "692  ", "post_office": "安来", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "エノシマチョウ", "alternates": []}');
-INSERT INTO office_data VALUES('6928601','{"jis": "32206", "kana": "ヒタチキンゾク カブシキカイシヤ ヤスギコウジヨウ", "name": "日立金属　株式会社　安来工場", "prefecture": "島根県", "city": "安来市", "neighborhood": "安来町", "banchi": "2107-2(安来郵便局私書箱第1号)", "postal_code": "6928601", "old_code": "692  ", "post_office": "安来", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "ヤスギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6928686','{"jis": "32206", "kana": "ヤスギシヤクシヨ", "name": "安来市役所", "prefecture": "島根県", "city": "安来市", "neighborhood": "安来町", "banchi": "878(安来郵便局私書箱第3号)", "postal_code": "6928686", "old_code": "692  ", "post_office": "安来", "type": "box", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ヤスギシ", "neighborhood_kana": "ヤスギチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6958577','{"jis": "32207", "kana": "カブシキガイシヤシチダキヨウイクケンキユウジヨ", "name": "株式会社　しちだ・教育研究所", "prefecture": "島根県", "city": "江津市", "neighborhood": "江津町", "banchi": "526-1", "postal_code": "6958577", "old_code": "695  ", "post_office": "江津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "ゴウツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6958585','{"jis": "32207", "kana": "キヨウドウクミアイ グリ-ンモ-ル", "name": "協同組合　グリーンモール", "prefecture": "島根県", "city": "江津市", "neighborhood": "嘉久志町", "banchi": "2306-30", "postal_code": "6958585", "old_code": "695  ", "post_office": "江津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "カクシチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6958501','{"jis": "32207", "kana": "ゴウツシヤクシヨ", "name": "江津市役所", "prefecture": "島根県", "city": "江津市", "neighborhood": "江津町", "banchi": "1016-4", "postal_code": "6958501", "old_code": "695  ", "post_office": "江津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "ゴウツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6958502','{"jis": "32207", "kana": "ゴウノカワコウトウガツコウ", "name": "江の川高等学校", "prefecture": "島根県", "city": "江津市", "neighborhood": "渡津町", "banchi": "1904-1", "postal_code": "6958502", "old_code": "695  ", "post_office": "江津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "ワタヅチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6958505','{"jis": "32207", "kana": "シヤカイフクシホウジン オンシザイダン シマネケンサイセイカイ ゴウツソウゴウビヨウイン", "name": "社会福祉法人　恩賜財団　島根県済生会　江津総合病院", "prefecture": "島根県", "city": "江津市", "neighborhood": "江津町", "banchi": "1016-37", "postal_code": "6958505", "old_code": "695  ", "post_office": "江津", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "ゴウツチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('6994298','{"jis": "32207", "kana": "イマイサンギヨウ カブシキガイシヤ", "name": "今井産業　株式会社", "prefecture": "島根県", "city": "江津市", "neighborhood": "桜江町川戸", "banchi": "472-1", "postal_code": "6994298", "old_code": "69942", "post_office": "市山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "シマネケン", "city_kana": "ゴウツシ", "neighborhood_kana": "サクラエチョウカワド", "alternates": []}');
@@ -138455,15 +138499,15 @@
 INSERT INTO office_data VALUES('7008515','{"jis": "33101", "kana": "カブシキガイシヤ ホテルグランヴイアオカヤマ", "name": "株式会社　ホテルグランヴィア岡山", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "駅元町", "banchi": "1-5", "postal_code": "7008515", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "エキモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7008561','{"jis": "33101", "kana": "カブシキガイシヤ マイカルオカヤマビブレ", "name": "株式会社　マイカル岡山ビブレ", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "幸町", "banchi": "7-6", "postal_code": "7008561", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "サイワイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7008620','{"jis": "33101", "kana": "カブシキガイシヤ ユメバンチ", "name": "株式会社　夢番地", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "中山下", "banchi": "1丁目10-10新田ビル6F", "postal_code": "7008620", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "ナカサンゲ", "alternates": []}');
 INSERT INTO office_data VALUES('7008508','{"jis": "33101", "kana": "カブシキガイシヤ リヨウビシステムズ", "name": "株式会社　両備システムズ", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "下石井", "banchi": "二丁目10番12号杜の街グレースオフィススクエア", "postal_code": "7008508", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "シモイシイ", "alternates": []}');
 INSERT INTO office_data VALUES('7008505','{"jis": "33101", "kana": "カワサキイカダイガクソウゴウイリヨウセンタ-", "name": "川崎医科大学総合医療センター", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "中山下", "banchi": "二丁目6番1号", "postal_code": "7008505", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "ナカサンゲ", "alternates": []}');
 INSERT INTO office_data VALUES('7008701','{"jis": "33101", "kana": "キハラコウギヨウ カブシキガイシヤ", "name": "木原興業　株式会社", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "田町", "banchi": "1丁目4-15(岡山中央郵便局私書箱第110号)", "postal_code": "7008701", "old_code": "700  ", "post_office": "岡山中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "タマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7008549','{"jis": "33101", "kana": "コ-ホクインサツ カブシキガイシヤ", "name": "コーホク印刷　株式会社", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "高柳東町", "banchi": "10-27", "postal_code": "7008549", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "タカヤナギヒガシマチ", "alternates": []}');
-INSERT INTO office_data VALUES('7008569','{"jis": "33101", "kana": "コクミンキヨウサイコ-プオカヤマスイシンホンブ", "name": "こくみん共済ｃｏｏｐ岡山推進本部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "駅元町", "banchi": "6番26号", "postal_code": "7008569", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "エキモトマチ", "alternates": []}');
+INSERT INTO office_data VALUES('7008569','{"jis": "33101", "kana": "コクミンキヨウサイコ-プオカヤマスイシンホンブ", "name": "こくみん共済ｃｏｏｐ岡山推進本部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "駅元町", "banchi": "6番26号", "postal_code": "7008569", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "エキモトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7008522','{"jis": "33101", "kana": "ザイダンホウジン シヤカイホケンケンコウジギヨウザイダン オカヤマケンシブ", "name": "財団法人　社会保険健康事業財団　岡山県支部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "磨屋町", "banchi": "10番20号磨屋町ビル5F", "postal_code": "7008522", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "トギヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7008567','{"jis": "33101", "kana": "シヤダンホウジン オカヤマケントラツクキヨウカイ", "name": "社団法人　岡山トラック協会", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "青江", "banchi": "1丁目22-33", "postal_code": "7008567", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "アオエ", "alternates": []}');
 INSERT INTO office_data VALUES('7008584','{"jis": "33101", "kana": "シンゴンシユウ ヤクシイン", "name": "真言宗　薬師院", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "磨屋町", "banchi": "2-18", "postal_code": "7008584", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "トギヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7008517','{"jis": "33101", "kana": "ジエイタイ オカヤマチホウレンラクブ", "name": "自衛隊　岡山地方連絡部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "下石井", "banchi": "1丁目4-1岡山第2合同庁舎2F", "postal_code": "7008517", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "シモイシイ", "alternates": []}');
 INSERT INTO office_data VALUES('7008614','{"jis": "33101", "kana": "スミクラ カブシキガイシヤ", "name": "スミクラ　株式会社", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "十日市中町", "banchi": "15番56号", "postal_code": "7008614", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "トウカイチナカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7008506','{"jis": "33101", "kana": "ゼンコクケンコウホケンキヨウカイ オカヤマシブ", "name": "全国健康保険協会　岡山支部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "本町", "banchi": "6-36第一セントラルビル", "postal_code": "7008506", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7008722','{"jis": "33101", "kana": "ゼンコクノウギヨウキヨクドウクミアイレンゴウカイ オカヤマケンホンブ", "name": "全国農業協同組合連合会　岡山県本部", "prefecture": "岡山県", "city": "岡山市北区", "neighborhood": "磨屋町", "banchi": "9-18-201", "postal_code": "7008722", "old_code": "700  ", "post_office": "岡山中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オカヤマケン", "city_kana": "オカヤマシキタク", "neighborhood_kana": "トギヤチョウ", "alternates": []}');
@@ -139412,15 +139456,15 @@
 INSERT INTO office_data VALUES('7478622','{"jis": "35206", "kana": "カブシキガイシヤ サンユウ", "name": "株式会社　三友", "prefecture": "山口県", "city": "防府市", "neighborhood": "駅南町", "banchi": "9-43(防府郵便局私書箱第25号)", "postal_code": "7478622", "old_code": "747  ", "post_office": "防府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "エキミナミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7478509','{"jis": "35206", "kana": "カブシキガイシヤ マルキユウ", "name": "株式会社　丸久", "prefecture": "山口県", "city": "防府市", "neighborhood": "大字江泊", "banchi": "1936", "postal_code": "7478509", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7478522','{"jis": "35206", "kana": "キヨウワハツコウコウギヨウ カブシキガイシヤ ホウフコウジヨウ", "name": "協和発酵工業　株式会社　防府工場", "prefecture": "山口県", "city": "防府市", "neighborhood": "協和町", "banchi": "1-1", "postal_code": "7478522", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "キョウワチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7478585','{"jis": "35206", "kana": "ケンセツシヨウヤマグチコウジジムシヨ", "name": "建設省山口工事事務所", "prefecture": "山口県", "city": "防府市", "neighborhood": "国衙", "banchi": "1丁目10-20", "postal_code": "7478585", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "コクガ", "alternates": []}');
 INSERT INTO office_data VALUES('7478567','{"jis": "35206", "kana": "コウクウジエイタイ ホウフキタキチ", "name": "航空自衛隊　防府北基地", "prefecture": "山口県", "city": "防府市", "neighborhood": "大字田島", "banchi": "無番地", "postal_code": "7478567", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7478555','{"jis": "35206", "kana": "コウクウジエイタイ ホウフミナミキチ", "name": "航空自衛隊　防府南基地", "prefecture": "山口県", "city": "防府市", "neighborhood": "大字田島", "banchi": "無番地", "postal_code": "7478555", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7478511','{"jis": "35206", "kana": "チホウドクリツギヨウセイホウジン ヤマグチケンリツビヨウインキコウ ヤマグチケンリツソウゴウイリヨウセンタ-", "name": "地方独立行政法人　山口県立病院機構　山口県立総合医療センター", "prefecture": "山口県", "city": "防府市", "neighborhood": "大字大崎", "banchi": "77番地", "postal_code": "7478511", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
-INSERT INTO office_data VALUES('7478533','{"jis": "35206", "kana": "ヒロシマコクゼイキヨクギヨウムセンタ-ホウフブンシツ", "name": "広島国税局業務センター防府分室", "prefecture": "山口県", "city": "防府市", "neighborhood": "寿町", "banchi": "6番39号防府地方合同庁舎", "postal_code": "7478533", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": true, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('7478533','{"jis": "35206", "kana": "ヒロシマコクゼイキヨクギヨウムセンタ-ホウフブンシツ", "name": "広島国税局業務センター防府分室", "prefecture": "山口県", "city": "防府市", "neighborhood": "寿町", "banchi": "6番39号防府地方合同庁舎", "postal_code": "7478533", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7478501','{"jis": "35206", "kana": "ホウフシヤクシヨ", "name": "防府市役所", "prefecture": "山口県", "city": "防府市", "neighborhood": "寿町", "banchi": "7-1", "postal_code": "7478501", "old_code": "747  ", "post_office": "防府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "コトブキチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7478611','{"jis": "35206", "kana": "ホウフゼイムシヨ", "name": "防府税務署", "prefecture": "山口県", "city": "防府市", "neighborhood": "緑町", "banchi": "1丁目2-12(防府郵便局私書箱第5号)", "postal_code": "7478611", "old_code": "747  ", "post_office": "防府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "ミドリマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7478686','{"jis": "35206", "kana": "ヤマグチギンコウホウフシテン", "name": "山口銀行　防府支店", "prefecture": "山口県", "city": "防府市", "neighborhood": "駅南町", "banchi": "10-1(防府郵便局私書箱第6号)", "postal_code": "7478686", "old_code": "747  ", "post_office": "防府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "ホウフシ", "neighborhood_kana": "エキミナミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7448601','{"jis": "35207", "kana": "カブシキガイシヤ ヒタチセイサクシヨ カサドジギヨウシヨ", "name": "株式会社　日立製作所　笠戸事業所", "prefecture": "山口県", "city": "下松市", "neighborhood": "大字東豊井", "banchi": "794(下松郵便局私書箱第1号)", "postal_code": "7448601", "old_code": "744  ", "post_office": "下松", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7448585','{"jis": "35207", "kana": "クダマツシヤクシヨ", "name": "下松市役所", "prefecture": "山口県", "city": "下松市", "neighborhood": "大手町", "banchi": "3丁目3-3", "postal_code": "7448585", "old_code": "744  ", "post_office": "下松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "クダマツシ", "neighborhood_kana": "オオテマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7448521','{"jis": "35207", "kana": "クダマツシヨウギヨウカイハツ カブシキガイシヤ", "name": "下松商業開発　株式会社", "prefecture": "山口県", "city": "下松市", "neighborhood": "中央町", "banchi": "21-3", "postal_code": "7448521", "old_code": "744  ", "post_office": "下松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "クダマツシ", "neighborhood_kana": "チュウオウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7448611','{"jis": "35207", "kana": "トウヨウコウハン カブシキガイシヤ クダマツコウジヨウ", "name": "東洋鋼鈑　株式会社　下松工場", "prefecture": "山口県", "city": "下松市", "neighborhood": "大字東豊井", "banchi": "1302-1(下松郵便局私書箱第13号)", "postal_code": "7448611", "old_code": "744  ", "post_office": "下松", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -139494,15 +139538,15 @@
 INSERT INTO office_data VALUES('7468666','{"jis": "35215", "kana": "ニツテツステンレス カブシキガイシヤ セイゾウホンブ シユウナンセイコウシヨ", "name": "日鉄ステンレス　株式会社　製造本部　周南製鋼所", "prefecture": "山口県", "city": "周南市", "neighborhood": "野村南町", "banchi": "4976番地(徳山郵便局私書箱第78号)", "postal_code": "7468666", "old_code": "746  ", "post_office": "徳山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "シュウナンシ", "neighborhood_kana": "ノムラミナミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7468601','{"jis": "35215", "kana": "ヤマグチギンコウ トンダシテン", "name": "山口銀行　富田支店", "prefecture": "山口県", "city": "周南市", "neighborhood": "政所", "banchi": "3丁目14-11(新南陽郵便局私書箱第3号)", "postal_code": "7468601", "old_code": "746  ", "post_office": "徳山", "type": "box", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "シュウナンシ", "neighborhood_kana": "マドコロ", "alternates": []}');
 INSERT INTO office_data VALUES('7568585','{"jis": "35216", "kana": "オノダシヨウギヨウカイハツ カブシキガイシヤ", "name": "小野田商業開発　株式会社", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "中川", "banchi": "6丁目4番1号", "postal_code": "7568585", "old_code": "756  ", "post_office": "小野田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "サンヨウオノダシ", "neighborhood_kana": "ナカガワ", "alternates": []}');
 INSERT INTO office_data VALUES('7568502','{"jis": "35216", "kana": "カブシキガイシヤ パオ", "name": "株式会社　パオ", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "大字西高泊", "banchi": "字烏帽子岩沖676番地9の1", "postal_code": "7568502", "old_code": "756  ", "post_office": "小野田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7568601','{"jis": "35216", "kana": "サンヨウオノダシヤクシヨ", "name": "山陽小野田市役所", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "日の出", "banchi": "1丁目1-1", "postal_code": "7568601", "old_code": "756  ", "post_office": "小野田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "サンヨウオノダシ", "neighborhood_kana": "ヒノデ", "alternates": []}');
 INSERT INTO office_data VALUES('7568602','{"jis": "35216", "kana": "シマダコウギヨウ", "name": "嶋田工業", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "大字西高泊", "banchi": "631-11(小野田郵便局私書箱第21号)", "postal_code": "7568602", "old_code": "756  ", "post_office": "小野田", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7568501','{"jis": "35216", "kana": "フジシヨウ カブシキガイシヤ", "name": "富士商　株式会社", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "稲荷町", "banchi": "10番23号", "postal_code": "7568501", "old_code": "756  ", "post_office": "小野田", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "サンヨウオノダシ", "neighborhood_kana": "イナリマチ", "alternates": []}');
-INSERT INTO office_data VALUES('7578585','{"jis": "35216", "kana": "エヌジエイコンポ-ネント カブシキガイシヤ サンヨウジギヨウシヨ", "name": "ＮＪコンポーネント　株式会社　山陽事業所", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "本町", "banchi": "5区", "postal_code": "7578585", "old_code": "757  ", "post_office": "厚狭", "type": "office", "multiple": false, "new": true, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+INSERT INTO office_data VALUES('7578585','{"jis": "35216", "kana": "エヌジエイコンポ-ネント カブシキガイシヤ サンヨウジギヨウシヨ", "name": "ＮＪコンポーネント　株式会社　山陽事業所", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "本町", "banchi": "5区", "postal_code": "7578585", "old_code": "757  ", "post_office": "厚狭", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7578634','{"jis": "35216", "kana": "サンヨウオノダシ サンヨウソウゴウジムシヨ", "name": "山陽小野田市　山陽総合事務所", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "大字鴨庄", "banchi": "94", "postal_code": "7578634", "old_code": "757  ", "post_office": "厚狭", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7578511','{"jis": "35216", "kana": "チヨウシユウサンギヨウ カブシキガイシヤ", "name": "長州産業　株式会社", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "", "banchi": "新山野井3740", "postal_code": "7578511", "old_code": "757  ", "post_office": "厚狭", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "サンヨウオノダシ", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7578686','{"jis": "35216", "kana": "ニホンカヤク カブシキガイシヤ アサコウジヨウ", "name": "日本化薬　株式会社　厚狭工場", "prefecture": "山口県", "city": "山陽小野田市", "neighborhood": "大字郡", "banchi": "2300(厚狭郵便局私書箱第1号)", "postal_code": "7578686", "old_code": "757  ", "post_office": "厚狭", "type": "box", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7422193','{"jis": "35305", "kana": "オオシマシヨウセンコウトウセンモンガツコウ", "name": "大島商船高等専門学校", "prefecture": "山口県", "city": "大島郡周防大島町", "neighborhood": "大字小松", "banchi": "1091-1", "postal_code": "7422193", "old_code": "74221", "post_office": "大島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7422192','{"jis": "35305", "kana": "スオウオオシマチヨウヤクバ", "name": "周防大島町役場", "prefecture": "山口県", "city": "大島郡周防大島町", "neighborhood": "大字小松", "banchi": "126番地2", "postal_code": "7422192", "old_code": "74221", "post_office": "大島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('7408501','{"jis": "35321", "kana": "ワキチヨウヤクバ", "name": "和木町役場", "prefecture": "山口県", "city": "玖珂郡和木町", "neighborhood": "和木", "banchi": "1丁目1-1", "postal_code": "7408501", "old_code": "740  ", "post_office": "岩国", "type": "office", "multiple": false, "new": false, "prefecture_kana": "ヤマグチケン", "city_kana": "クガグンワキチョウ", "neighborhood_kana": "ワキ", "alternates": []}');
 INSERT INTO office_data VALUES('7421598','{"jis": "35343", "kana": "タイコウキカイコウギヨウ カブシキガイシヤ", "name": "大晃機械工業　株式会社", "prefecture": "山口県", "city": "熊毛郡田布施町", "neighborhood": "大字下田布施", "banchi": "209-1", "postal_code": "7421598", "old_code": "74215", "post_office": "田布施", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
@@ -139674,15 +139718,15 @@
 INSERT INTO office_data VALUES('7710287','{"jis": "36402", "kana": "シコクカコウキ カブシキガイシヤ", "name": "四国化工機　（株）", "prefecture": "徳島県", "city": "板野郡北島町", "neighborhood": "太郎八須", "banchi": "字西ノ川10-1", "postal_code": "7710287", "old_code": "77102", "post_office": "北島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンキタジマチョウ", "neighborhood_kana": "タロウハチズ", "alternates": []}');
 INSERT INTO office_data VALUES('7710288','{"jis": "36402", "kana": "シコクカセイコウギヨウ カブシキガイシヤ トクシマダイニコウジヨウ", "name": "四国化成工業　（株）　徳島第二工場", "prefecture": "徳島県", "city": "板野郡北島町", "neighborhood": "江尻", "banchi": "字内中須1", "postal_code": "7710288", "old_code": "77102", "post_office": "北島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンキタジマチョウ", "neighborhood_kana": "エジリ", "alternates": []}');
 INSERT INTO office_data VALUES('7710289','{"jis": "36402", "kana": "セイカツキヨウドウクミアイ トクシマセイキヨウ", "name": "生活協同組合　とくしま生協", "prefecture": "徳島県", "city": "板野郡北島町", "neighborhood": "中村", "banchi": "字東堤ノ内30-3", "postal_code": "7710289", "old_code": "77102", "post_office": "北島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンキタジマチョウ", "neighborhood_kana": "ナカムラ", "alternates": []}');
 INSERT INTO office_data VALUES('7710283','{"jis": "36402", "kana": "ハ-トフルカワウチ カブシキガイシヤ", "name": "はーとふる川内　株式会社", "prefecture": "徳島県", "city": "板野郡北島町", "neighborhood": "高房", "banchi": "字居内1-1", "postal_code": "7710283", "old_code": "77102", "post_office": "北島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンキタジマチョウ", "neighborhood_kana": "タカボウ", "alternates": []}');
 INSERT INTO office_data VALUES('7711292','{"jis": "36403", "kana": "アイズミチヨウヤクバ", "name": "藍住町役場", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "奥野", "banchi": "字矢上前52-1", "postal_code": "7711292", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "オクノ", "alternates": []}');
 INSERT INTO office_data VALUES('7711297','{"jis": "36403", "kana": "カネコミソ カブシキガイシヤ", "name": "かねこみそ　（株）", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "奥野", "banchi": "字乾81-2", "postal_code": "7711297", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "オクノ", "alternates": []}');
 INSERT INTO office_data VALUES('7711294','{"jis": "36403", "kana": "カブシキガイシヤ ジエイテクト トクシマコウジヨウ", "name": "（株）　ジェイテクト　徳島工場", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "奥野", "banchi": "字山畑1", "postal_code": "7711294", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "オクノ", "alternates": []}');
-INSERT INTO office_data VALUES('7711295','{"jis": "36403", "kana": "カブシキガイシヤ ジエイテクトシ-リングテクノ", "name": "（株）　ジェイテクトシーリングテクノ", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "笠木", "banchi": "字西野39", "postal_code": "7711295", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": true, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "カサギ", "alternates": []}');
+INSERT INTO office_data VALUES('7711295','{"jis": "36403", "kana": "カブシキガイシヤ ジエイテクトシ-リングテクノ", "name": "（株）　ジェイテクトシーリングテクノ", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "笠木", "banchi": "字西野39", "postal_code": "7711295", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "カサギ", "alternates": []}');
 INSERT INTO office_data VALUES('7711289','{"jis": "36403", "kana": "カブシキガイシヤ メデイング", "name": "（株）　メディング", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "住吉", "banchi": "字神蔵5-1", "postal_code": "7711289", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "スミヨシ", "alternates": []}');
 INSERT INTO office_data VALUES('7711298','{"jis": "36403", "kana": "ヤマクシヨクヒン カブシキガイシヤ", "name": "ヤマク食品　（株）", "prefecture": "徳島県", "city": "板野郡藍住町", "neighborhood": "奥野", "banchi": "字乾170", "postal_code": "7711298", "old_code": "77112", "post_office": "藍住", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンアイズミチョウ", "neighborhood_kana": "オクノ", "alternates": []}');
 INSERT INTO office_data VALUES('7790192','{"jis": "36404", "kana": "イタノチヨウヤクバ", "name": "板野町役場", "prefecture": "徳島県", "city": "板野郡板野町", "neighborhood": "吹田", "banchi": "字町南22-2", "postal_code": "7790192", "old_code": "77901", "post_office": "板野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンイタノチョウ", "neighborhood_kana": "フキタ", "alternates": []}');
 INSERT INTO office_data VALUES('7790195','{"jis": "36404", "kana": "オオツカセイヤク カブシキガイシヤ トクシマイタノコウジヨウ", "name": "大塚製薬　株式会社　徳島板野工場", "prefecture": "徳島県", "city": "板野郡板野町", "neighborhood": "松谷", "banchi": "字シシトキ南13", "postal_code": "7790195", "old_code": "77901", "post_office": "板野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンイタノチョウ", "neighborhood_kana": "マツダニ", "alternates": []}');
 INSERT INTO office_data VALUES('7790193','{"jis": "36404", "kana": "コクリツリヨウヨウシヨ ヒガシトクシマビヨウイン", "name": "国立療養所　東徳島病院", "prefecture": "徳島県", "city": "板野郡板野町", "neighborhood": "大寺", "banchi": "字大向北1-1", "postal_code": "7790193", "old_code": "77901", "post_office": "板野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンイタノチョウ", "neighborhood_kana": "オオテラ", "alternates": []}');
 INSERT INTO office_data VALUES('7790194','{"jis": "36404", "kana": "フジフアニチア カブシキガイシヤ", "name": "冨士ファニチア　株式会社", "prefecture": "徳島県", "city": "板野郡板野町", "neighborhood": "矢武", "banchi": "字神木1-1", "postal_code": "7790194", "old_code": "77901", "post_office": "板野", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンイタノチョウ", "neighborhood_kana": "ヤタケ", "alternates": []}');
 INSERT INTO office_data VALUES('7711392','{"jis": "36405", "kana": "カミイタチヨウヤクバ", "name": "上板町役場", "prefecture": "徳島県", "city": "板野郡上板町", "neighborhood": "七條", "banchi": "字経塚42", "postal_code": "7711392", "old_code": "77113", "post_office": "上板", "type": "office", "multiple": false, "new": false, "prefecture_kana": "トクシマケン", "city_kana": "イタノグンカミイタチョウ", "neighborhood_kana": "シチジョウ", "alternates": []}');
@@ -140038,26 +140082,26 @@
 INSERT INTO office_data VALUES('7918512','{"jis": "38201", "kana": "エヒメトヨペツト カブシキガイシヤ", "name": "愛媛トヨペット　株式会社", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "空港通", "banchi": "5丁目7-9", "postal_code": "7918512", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クウコウドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7918527','{"jis": "38201", "kana": "オイエサンギヨウ カブシキガイシヤ マツヤマエイギヨウシヨ", "name": "尾家産業　（株）　松山営業所", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "久万ノ台", "banchi": "577-1", "postal_code": "7918527", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クマノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('7918555','{"jis": "38201", "kana": "オオゾラビヨウイン", "name": "おおぞら病院", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "六軒家町", "banchi": "4-20", "postal_code": "7918555", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "ロッケンヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918675','{"jis": "38201", "kana": "カブシキカイシヤ マツミヤ", "name": "株式会社　松宮", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "問屋町", "banchi": "6-26(松山問屋町郵便局私書箱第26号)", "postal_code": "7918675", "old_code": "791  ", "post_office": "松山西", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "トイヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918524','{"jis": "38201", "kana": "カブシキガイシヤ アテツクス", "name": "（株）　アテックス", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "衣山", "banchi": "1丁目2-5", "postal_code": "7918524", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キヌヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('7918671','{"jis": "38201", "kana": "カブシキガイシヤ イツシキホンテン", "name": "（株）　一色本店", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "問屋町", "banchi": "4-28(松山問屋町郵便局私書箱第1号)", "postal_code": "7918671", "old_code": "791  ", "post_office": "松山西", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "トイヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918603','{"jis": "38201", "kana": "カブシキガイシヤ エヒメインリヨウ", "name": "株式会社　えひめ飲料", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "安城寺町", "banchi": "478(松山西郵便局私書箱第12号)", "postal_code": "7918603", "old_code": "791  ", "post_office": "松山西", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "アンジョウジマチ", "alternates": []}');
+INSERT INTO office_data VALUES('7918525','{"jis": "38201", "kana": "カブシキガイシヤ オオサカソ-ダ マツヤマコウジヨウ", "name": "株式会社　大阪ソーダ　松山工場", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "北吉田町", "banchi": "77番地", "postal_code": "7918525", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": true, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キタヨシダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918672','{"jis": "38201", "kana": "カブシキガイシヤ カナツクス", "name": "株式会社　カナックス", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "姫原", "banchi": "3丁目5番11号", "postal_code": "7918672", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "ヒメバラ", "alternates": []}');
 INSERT INTO office_data VALUES('7918538','{"jis": "38201", "kana": "カブシキガイシヤ ジヨウセイ", "name": "（株）　城西", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "富久町", "banchi": "422-7", "postal_code": "7918538", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "トミヒサマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918528','{"jis": "38201", "kana": "カブシキガイシヤ ニホンブング", "name": "（株）日本文具", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "中央", "banchi": "1丁目4-2", "postal_code": "7918528", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918505','{"jis": "38201", "kana": "カブシキガイシヤ ハ-ト", "name": "株式会社　ハート", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "大可賀", "banchi": "3丁目150番地8", "postal_code": "7918505", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "オオカガ", "alternates": []}');
 INSERT INTO office_data VALUES('7918507','{"jis": "38201", "kana": "カブシキガイシヤ パステムマツザワ", "name": "（株）　パステムマツザワ", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "久万ノ台", "banchi": "689", "postal_code": "7918507", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クマノダイ", "alternates": []}');
 INSERT INTO office_data VALUES('7918501','{"jis": "38201", "kana": "ガツコウホウジン アイコウガクエン", "name": "学校法人　愛光学園", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "衣山", "banchi": "5丁目1610-1", "postal_code": "7918501", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キヌヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('7918508','{"jis": "38201", "kana": "キタシコクシヨウジ カブシキガイシヤ", "name": "北四国商事　（株）", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "南斎院町", "banchi": "345", "postal_code": "7918508", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "ミナミサヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918516','{"jis": "38201", "kana": "コスモマツヤマセキユ カブシキガイシヤ", "name": "コスモ松山石油　（株）", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "大可賀", "banchi": "3丁目580", "postal_code": "7918516", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "オオカガ", "alternates": []}');
 INSERT INTO office_data VALUES('7918535','{"jis": "38201", "kana": "コマツカスタマ-サポ-ト カブシキガイシヤ", "name": "コマツカスタマーサポート　株式会社", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "高岡町", "banchi": "151", "postal_code": "7918535", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "タカオカマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918510','{"jis": "38201", "kana": "シコクメイテツウンユ カブシキガイシヤ", "name": "四国名鉄運輸　株式会社", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "空港通", "banchi": "4丁目5番5号", "postal_code": "7918510", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クウコウドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7918517','{"jis": "38201", "kana": "ダイキ カブシキガイシヤ", "name": "ダイキ　株式会社", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "美沢", "banchi": "1丁目9-1", "postal_code": "7918517", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "ミサワ", "alternates": []}');
-INSERT INTO office_data VALUES('7918525','{"jis": "38201", "kana": "ダイソ- カブシキガイシヤ マツヤマコウジヨウ", "name": "ダイソー　株式会社　松山工場", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "北吉田町", "banchi": "77", "postal_code": "7918525", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キタヨシダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918531','{"jis": "38201", "kana": "ダイヤアルミ カブシキガイシヤ", "name": "ダイヤアルミ　（株）", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "安城寺町", "banchi": "571", "postal_code": "7918531", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "アンジョウジマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918513','{"jis": "38201", "kana": "テイ-エムテイ-マシナリ- カブシキガイシヤ マツヤマコウジヨウ", "name": "ＴＭＴマシナリー　株式会社　松山工場", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "北吉田町", "banchi": "77番地", "postal_code": "7918513", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キタヨシダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918530','{"jis": "38201", "kana": "テイジン カブシキガイシヤ マツヤマジギヨウシヨ", "name": "帝人　（株）　松山事業所", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "北吉田町", "banchi": "77", "postal_code": "7918530", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "キタヨシダマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918536','{"jis": "38201", "kana": "テイジンカブシキカイシヤ マツヤマジギヨウシヨ", "name": "帝人株式会社　松山事業所", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "西垣生町", "banchi": "2-3-45", "postal_code": "7918536", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "ニシハブマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7918506','{"jis": "38201", "kana": "トウシバフアイナンス カブシキガイシヤ エヒメエイギヨウシヨ", "name": "東芝ファイナンス　（株）　愛媛営業所", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "空港通", "banchi": "5丁目9-1", "postal_code": "7918506", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クウコウドオリ", "alternates": []}');
 INSERT INTO office_data VALUES('7918511','{"jis": "38201", "kana": "トヨタカロ-ラエヒメ カブシキガイシヤ", "name": "トヨタカローラ愛媛　（株）", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "中央", "banchi": "1丁目16-5", "postal_code": "7918511", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "チュウオウ", "alternates": []}');
 INSERT INTO office_data VALUES('7918502','{"jis": "38201", "kana": "トラスコナカヤマ カブシキガイシヤ マツヤマエイギヨウシヨ", "name": "トラスコ中山　株式会社　松山営業所", "prefecture": "愛媛県", "city": "松山市", "neighborhood": "久万ノ台", "banchi": "1068番4", "postal_code": "7918502", "old_code": "791  ", "post_office": "松山西", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "マツヤマシ", "neighborhood_kana": "クマノダイ", "alternates": []}');
@@ -140159,15 +140203,15 @@
 INSERT INTO office_data VALUES('7991198','{"jis": "38206", "kana": "サイジヨウシヤクシヨ コマツソウゴウシシヨ", "name": "西条市役所　小松総合支所", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "小松町新屋敷", "banchi": "甲496", "postal_code": "7991198", "old_code": "79911", "post_office": "小松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "コマツチョウシンヤシキ", "alternates": []}');
 INSERT INTO office_data VALUES('7991392','{"jis": "38206", "kana": "カブシキガイシヤ タクボコウギヨウシヨ", "name": "株式会社　田窪工業所", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "北条", "banchi": "962-7(東予郵便局私書箱第22号)", "postal_code": "7991392", "old_code": "79913", "post_office": "東予", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "ホウジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7991394','{"jis": "38206", "kana": "サイジヨウシヤクシヨ トウヨソウゴウシシヨ", "name": "西条市役所　東予総合支所", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "周布", "banchi": "349-1(東予郵便局私書箱第10号)", "postal_code": "7991394", "old_code": "79913", "post_office": "東予", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "シュウ", "alternates": []}');
 INSERT INTO office_data VALUES('7991395','{"jis": "38206", "kana": "シコクカイハツフエリ- カブシキガイシヤ", "name": "四国開発フェリー　株式会社", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "今在家", "banchi": "1500-2", "postal_code": "7991395", "old_code": "79913", "post_office": "東予", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "イマザイケ", "alternates": []}');
 INSERT INTO office_data VALUES('7991393','{"jis": "38206", "kana": "スミトモジユウキカイコウギヨウ カブシキガイシヤ", "name": "住友重機械工業　株式会社", "prefecture": "愛媛県", "city": "西条市", "neighborhood": "今在家", "banchi": "1501", "postal_code": "7991393", "old_code": "79913", "post_office": "東予", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "サイジョウシ", "neighborhood_kana": "イマザイケ", "alternates": []}');
 INSERT INTO office_data VALUES('7958504','{"jis": "38207", "kana": "エヒメケンナンヨチホウキヨクオオズチヨウシヤ", "name": "愛媛県南予地方局大洲庁舎", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "田口", "banchi": "甲425-1", "postal_code": "7958504", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "タノクチ", "alternates": []}');
 INSERT INTO office_data VALUES('7958502','{"jis": "38207", "kana": "エヒメケンリツ オオズコウトウガツコウ", "name": "愛媛県立　大洲高等学校", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "大洲", "banchi": "737", "postal_code": "7958502", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "オオズ", "alternates": []}');
-INSERT INTO office_data VALUES('7958506','{"jis": "38207", "kana": "エヒメタイキノウギヨウキヨウドウクミアイ ホンシヨ", "name": "愛媛たいき農業協同組合　本所", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "東大洲", "banchi": "1582番地", "postal_code": "7958506", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": true, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "ヒガシオオズ", "alternates": []}');
+INSERT INTO office_data VALUES('7958506','{"jis": "38207", "kana": "エヒメタイキノウギヨウキヨウドウクミアイ ホンシヨ", "name": "愛媛たいき農業協同組合　本所", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "東大洲", "banchi": "1582番地", "postal_code": "7958506", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "ヒガシオオズ", "alternates": []}');
 INSERT INTO office_data VALUES('7958510','{"jis": "38207", "kana": "オオズキネンビヨウイン", "name": "大洲記念病院", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "徳森", "banchi": "1512-1", "postal_code": "7958510", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "トクノモリ", "alternates": []}');
 INSERT INTO office_data VALUES('7958601','{"jis": "38207", "kana": "オオズシヤクシヨ", "name": "大洲市役所", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "大洲", "banchi": "690-1(大洲郵便局私書箱第7号)", "postal_code": "7958601", "old_code": "795  ", "post_office": "大洲", "type": "box", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "オオズ", "alternates": []}');
 INSERT INTO office_data VALUES('7958507','{"jis": "38207", "kana": "オオズチユウオウビヨウイン", "name": "大洲中央病院", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "東大洲", "banchi": "5", "postal_code": "7958507", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "ヒガシオオズ", "alternates": []}');
 INSERT INTO office_data VALUES('7958505','{"jis": "38207", "kana": "キタイシカイビヨウイン", "name": "喜多医師会病院", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "東大洲", "banchi": "1563番地1", "postal_code": "7958505", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "ヒガシオオズ", "alternates": []}');
 INSERT INTO office_data VALUES('7958501','{"jis": "38207", "kana": "シリツオオズビヨウイン", "name": "市立大洲病院", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "西大洲", "banchi": "甲570", "postal_code": "7958501", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "ニシオオズ", "alternates": []}');
 INSERT INTO office_data VALUES('7958603','{"jis": "38207", "kana": "ニシダコウサン", "name": "西田興産", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "徳森", "banchi": "248", "postal_code": "7958603", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "トクノモリ", "alternates": []}');
 INSERT INTO office_data VALUES('7958508','{"jis": "38207", "kana": "マルサンサンギヨウ カブシキガイシヤ", "name": "丸三産業　株式会社", "prefecture": "愛媛県", "city": "大洲市", "neighborhood": "徳森", "banchi": "字渡リ1349", "postal_code": "7958508", "old_code": "795  ", "post_office": "大洲", "type": "office", "multiple": false, "new": false, "prefecture_kana": "エヒメケン", "city_kana": "オオズシ", "neighborhood_kana": "トクノモリ", "alternates": []}');
@@ -140253,15 +140297,14 @@
 INSERT INTO office_data VALUES('7808561','{"jis": "39201", "kana": "カブシキカイシヤ コウチシンハンキユウホテル", "name": "株式会社　高知新阪急ホテル", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "4丁目2番地50号", "postal_code": "7808561", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808676','{"jis": "39201", "kana": "カブシキガイシヤ アワギンコウ コウチシテン", "name": "株式会社　阿波銀行　高知支店", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "4丁目2-52", "postal_code": "7808676", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808527','{"jis": "39201", "kana": "カブシキガイシヤ エヌ・シ-・ビ-", "name": "株式会社　エヌ・シー・ビー", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "2丁目3-4", "postal_code": "7808527", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808540','{"jis": "39201", "kana": "カブシキガイシヤ キタムラ", "name": "株式会社　キタムラ", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "4-1-16", "postal_code": "7808540", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808602','{"jis": "39201", "kana": "カブシキガイシヤ コウチギンコウ", "name": "株式会社　高知銀行", "prefecture": "高知県", "city": "高知市", "neighborhood": "堺町", "banchi": "2-24(高知中央郵便局私書箱第13号)", "postal_code": "7808602", "old_code": "780  ", "post_office": "高知中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "サカイマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808666','{"jis": "39201", "kana": "カブシキガイシヤ コウチシンブンキギヨウ", "name": "株式会社　高知新聞企業", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "3丁目2-15", "postal_code": "7808666", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808572','{"jis": "39201", "kana": "カブシキガイシヤ コウチシンブンシヤ", "name": "株式会社　高知新聞社", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "3丁目2-15", "postal_code": "7808572", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
-INSERT INTO office_data VALUES('7808662','{"jis": "39201", "kana": "カブシキガイシヤ コウチシンブンシヤ (パブリシテイ)", "name": "株式会社　高知新聞社　（パブリシティ）", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "3丁目2-15", "postal_code": "7808662", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808566','{"jis": "39201", "kana": "カブシキガイシヤ コウチダイマル", "name": "株式会社　高知大丸", "prefecture": "高知県", "city": "高知市", "neighborhood": "帯屋町", "banchi": "1丁目6-1", "postal_code": "7808566", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "オビヤマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808550','{"jis": "39201", "kana": "カブシキガイシヤ コウチホウソウ", "name": "株式会社　高知放送", "prefecture": "高知県", "city": "高知市", "neighborhood": "本町", "banchi": "3丁目2-8", "postal_code": "7808550", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808517','{"jis": "39201", "kana": "カブシキガイシヤ サニ-マ-ト", "name": "株式会社　サニーマート", "prefecture": "高知県", "city": "高知市", "neighborhood": "山手町", "banchi": "81番", "postal_code": "7808517", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ヤマテチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7808663','{"jis": "39201", "kana": "カブシキガイシヤ サンスイエン", "name": "株式会社　三翠園", "prefecture": "高知県", "city": "高知市", "neighborhood": "鷹匠町", "banchi": "1-3-35", "postal_code": "7808663", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "タカジョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('7808605','{"jis": "39201", "kana": "カブシキガイシヤ シコクギンコウ", "name": "株式会社　四国銀行", "prefecture": "高知県", "city": "高知市", "neighborhood": "南はりまや町", "banchi": "1丁目1-1(高知中央郵便局私書箱第5号)", "postal_code": "7808605", "old_code": "780  ", "post_office": "高知中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "ミナミハリマヤチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7808787','{"jis": "39201", "kana": "カブシキガイシヤ ユウチヨギンコウ コウチチイキセンタ-", "name": "株式会社　ゆうちょ銀行　高知地域センター", "prefecture": "高知県", "city": "高知市", "neighborhood": "駅前町", "banchi": "3-20ジブラルタ生命高知ビル9階", "postal_code": "7808787", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "エキマエチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('7808536','{"jis": "39201", "kana": "コウチケン コクミンケンコウホケンダンタイレンゴウカイ", "name": "高知県　国民健康保険団体連合会", "prefecture": "高知県", "city": "高知市", "neighborhood": "丸ノ内", "banchi": "2丁目6-5", "postal_code": "7808536", "old_code": "780  ", "post_office": "高知中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "コウチケン", "city_kana": "コウチシ", "neighborhood_kana": "マルノウチ", "alternates": []}');
@@ -140416,15 +140459,15 @@
 INSERT INTO office_data VALUES('8088585','{"jis": "40103", "kana": "シヤダンホウジン ワカマツホウジンカイ", "name": "社団法人　若松法人会", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "本町", "banchi": "1丁目13-15", "postal_code": "8088585", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8088588','{"jis": "40103", "kana": "シンワコウバン", "name": "信和鋼板", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "大字安瀬", "banchi": "8-4", "postal_code": "8088588", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8088514','{"jis": "40103", "kana": "セイワコウギヨウ カブシキガイシヤ キユウシユウシテン", "name": "清和鋼業　株式会社　九州支店", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "北浜", "banchi": "1丁目7-2", "postal_code": "8088514", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "キタハマ", "alternates": []}');
 INSERT INTO office_data VALUES('8088502','{"jis": "40103", "kana": "ツルマルカイウン カブシキガイシヤ", "name": "鶴丸海運　株式会社", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "本町", "banchi": "1丁目5-11", "postal_code": "8088502", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ホンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8088505','{"jis": "40103", "kana": "トウコウシヨクヒン カブシキガイシヤ", "name": "東紅食品　株式会社", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "浜町", "banchi": "1丁目19-11", "postal_code": "8088505", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ハママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8088550','{"jis": "40103", "kana": "フジボウエキ カブシキガイシヤ", "name": "不二貿易　株式会社", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "大字安瀬", "banchi": "64-36", "postal_code": "8088550", "old_code": "808  ", "post_office": "若松", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8088606','{"jis": "40103", "kana": "ワカマツゼイムシヨ", "name": "若松税務署", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "本町", "banchi": "1-14-12(若松郵便局私書箱第34号)", "postal_code": "8088606", "old_code": "808  ", "post_office": "若松", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ホンマチ", "alternates": []}');
-INSERT INTO office_data VALUES('8080196','{"jis": "40103", "kana": "キユウシユウコウギヨウダイガクダイガクイン セイメイタイコウガクケンキユウカ", "name": "九州工業大学大学院　生命体工学研究科", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "ひびきの", "banchi": "1-1", "postal_code": "8080196", "old_code": "80801", "post_office": "二島", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ヒビキノ", "alternates": []}');
+INSERT INTO office_data VALUES('8080196','{"jis": "40103", "kana": "キユウシユウコウギヨウダイガクダイガクイン セイメイタイコウガクケンキユウカ", "name": "九州工業大学大学院　生命体工学研究科", "prefecture": "福岡県", "city": "北九州市若松区", "neighborhood": "ひびきの", "banchi": "2-4", "postal_code": "8080196", "old_code": "80801", "post_office": "二島", "type": "office", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシワカマツク", "neighborhood_kana": "ヒビキノ", "alternates": []}');
 INSERT INTO office_data VALUES('8048520','{"jis": "40105", "kana": "アサヒガラス カブシキガイシヤ キタキユウシユウコウジヨウ", "name": "旭硝子　株式会社　北九州工場", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "牧山", "banchi": "5丁目1-1", "postal_code": "8048520", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシトバタク", "neighborhood_kana": "マキヤマ", "alternates": []}');
 INSERT INTO office_data VALUES('8048558','{"jis": "40105", "kana": "ガツコウホウジン メイジガクエン", "name": "学校法人　明治学園", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "仙水町", "banchi": "5-1", "postal_code": "8048558", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシトバタク", "neighborhood_kana": "センスイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8048510','{"jis": "40105", "kana": "キタキユウシユウシ トバタクヤクシヨ", "name": "北九州市　戸畑区役所", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "千防", "banchi": "1丁目1-1", "postal_code": "8048510", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシトバタク", "neighborhood_kana": "センボウ", "alternates": []}');
 INSERT INTO office_data VALUES('8048550','{"jis": "40105", "kana": "キユウシユウコウギヨウダイガク", "name": "九州工業大学", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "仙水町", "banchi": "1-1", "postal_code": "8048550", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシトバタク", "neighborhood_kana": "センスイチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8048539','{"jis": "40105", "kana": "サンキユウ カブシキガイシヤ キタキユウシユウシテン", "name": "山九　株式会社　北九州支店", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "大字中原", "banchi": "先の浜46-51先の浜ビル4F", "postal_code": "8048539", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8048538','{"jis": "40105", "kana": "サンキユウ カブシキガイシヤ ヤハタシテン", "name": "山九　株式会社　八幡支店", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "大字中原", "banchi": "先の浜46-51先の浜ビル", "postal_code": "8048538", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('8048601','{"jis": "40105", "kana": "トウヨウセイカン カブシキガイシヤ トバタコウジヨウ", "name": "東洋製罐　株式会社　戸畑工場", "prefecture": "福岡県", "city": "北九州市戸畑区", "neighborhood": "銀座", "banchi": "2丁目9-3", "postal_code": "8048601", "old_code": "804  ", "post_office": "戸畑", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "キタキュウシュウシトバタク", "neighborhood_kana": "ギンザ", "alternates": []}');
@@ -141113,15 +141156,15 @@
 INSERT INTO office_data VALUES('8114198','{"jis": "40220", "kana": "トウカイダイガク フクオカタンキダイガク", "name": "東海大学　福岡短期大学", "prefecture": "福岡県", "city": "宗像市", "neighborhood": "田久", "banchi": "1丁目9-1", "postal_code": "8114198", "old_code": "81141", "post_office": "宗像", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ムナカタシ", "neighborhood_kana": "タク", "alternates": []}');
 INSERT INTO office_data VALUES('8114192','{"jis": "40220", "kana": "フクオカキヨウイクダイガク", "name": "福岡教育大学", "prefecture": "福岡県", "city": "宗像市", "neighborhood": "赤間文教町", "banchi": "1番1号", "postal_code": "8114192", "old_code": "81141", "post_office": "宗像", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ムナカタシ", "neighborhood_kana": "アカマブンキョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8180193','{"jis": "40221", "kana": "ガツコウホウジン キユウシユウガクエン フクオカジヨシタンキダイガク", "name": "学校法人　九州学園　福岡女子短期大学", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "五条", "banchi": "4丁目16-1", "postal_code": "8180193", "old_code": "81801", "post_office": "太宰府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "ゴジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8180194','{"jis": "40221", "kana": "ダイイチフクシダイガク", "name": "第一福祉大学", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "五条", "banchi": "3丁目10-10", "postal_code": "8180194", "old_code": "81801", "post_office": "太宰府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "ゴジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8180198','{"jis": "40221", "kana": "ダザイフシヤクシヨ", "name": "太宰府市役所", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "観世音寺", "banchi": "1丁目1-1(太宰府郵便局私書箱第3号)", "postal_code": "8180198", "old_code": "81801", "post_office": "太宰府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "カンゼオンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8180195','{"jis": "40221", "kana": "ダザイフテンマングウ", "name": "太宰府天満宮", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "宰府", "banchi": "4丁目7-1(太宰府郵便局私書箱第1号)", "postal_code": "8180195", "old_code": "81801", "post_office": "太宰府", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "サイフ", "alternates": []}');
 INSERT INTO office_data VALUES('8180192','{"jis": "40221", "kana": "チクシジヨガクエンダイガク チクシジヨガクエンタンキダイガク", "name": "筑紫女学園大学　筑紫女学園短期大学", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "石坂", "banchi": "2丁目12-1", "postal_code": "8180192", "old_code": "81801", "post_office": "太宰府", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "イシザカ", "alternates": []}');
-INSERT INTO office_data VALUES('8180197','{"jis": "40221", "kana": "ニホンケイザイダイガク・フクオカコドモタンキダイガク", "name": "日本経済大学・福岡こども短期大学", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "五条", "banchi": "3丁目11-25(筑紫野郵便局私書箱第17号)", "postal_code": "8180197", "old_code": "81801", "post_office": "筑紫野", "type": "box", "multiple": false, "new": true, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "ゴジョウ", "alternates": []}');
+INSERT INTO office_data VALUES('8180197','{"jis": "40221", "kana": "ニホンケイザイダイガク・フクオカコドモタンキダイガク", "name": "日本経済大学・福岡こども短期大学", "prefecture": "福岡県", "city": "太宰府市", "neighborhood": "五条", "banchi": "3丁目11-25(筑紫野郵便局私書箱第17号)", "postal_code": "8180197", "old_code": "81801", "post_office": "筑紫野", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "ダザイフシ", "neighborhood_kana": "ゴジョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8113197','{"jis": "40223", "kana": "カブシキガイシヤ セイコウデンキセイサクシヨ", "name": "株式会社　正興電機製作所", "prefecture": "福岡県", "city": "古賀市", "neighborhood": "天神", "banchi": "3丁目20-1(古賀郵便局私書箱第2号)", "postal_code": "8113197", "old_code": "81131", "post_office": "古賀", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "コガシ", "neighborhood_kana": "テンジン", "alternates": []}');
 INSERT INTO office_data VALUES('8113192','{"jis": "40223", "kana": "コガシヤクシヨ", "name": "古賀市役所", "prefecture": "福岡県", "city": "古賀市", "neighborhood": "駅東", "banchi": "1丁目1-1", "postal_code": "8113192", "old_code": "81131", "post_office": "古賀", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "コガシ", "neighborhood_kana": "エキヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('8113195','{"jis": "40223", "kana": "コクリツビヨウインキコウ フクオカヒガシイリヨウセンタ-", "name": "国立病院機構　福岡東医療センタ－", "prefecture": "福岡県", "city": "古賀市", "neighborhood": "千鳥", "banchi": "1丁目1-1", "postal_code": "8113195", "old_code": "81131", "post_office": "古賀", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "コガシ", "neighborhood_kana": "チドリ", "alternates": []}');
 INSERT INTO office_data VALUES('8113193','{"jis": "40223", "kana": "セイブデンキ カブシキガイシヤ", "name": "西部電機　株式会社", "prefecture": "福岡県", "city": "古賀市", "neighborhood": "駅東", "banchi": "3丁目3-1(古賀郵便局私書箱第1号)", "postal_code": "8113193", "old_code": "81131", "post_office": "古賀", "type": "box", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "コガシ", "neighborhood_kana": "エキヒガシ", "alternates": []}');
 INSERT INTO office_data VALUES('8113198','{"jis": "40223", "kana": "ヤマサキセイパン カブシキガイシヤ フクオカコウジヨウ", "name": "山崎製パン　株式会社　福岡工場", "prefecture": "福岡県", "city": "古賀市", "neighborhood": "古賀", "banchi": "69", "postal_code": "8113198", "old_code": "81131", "post_office": "古賀", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "コガシ", "neighborhood_kana": "コガ", "alternates": []}');
 INSERT INTO office_data VALUES('8113295','{"jis": "40224", "kana": "イリヨウホウジン ケイアイカイ フクマビヨウイン", "name": "医療法人　恵愛会　福間病院", "prefecture": "福岡県", "city": "福津市", "neighborhood": "花見が浜", "banchi": "1丁目5-1", "postal_code": "8113295", "old_code": "81132", "post_office": "福間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクツシ", "neighborhood_kana": "ハナミガハマ", "alternates": []}');
 INSERT INTO office_data VALUES('8113298','{"jis": "40224", "kana": "シヤカイイリヨウホウジンスイコウカイ ムナカタスイコウカイソウゴウビヨウイン", "name": "社会医療法人水光会　宗像水光会総合病院", "prefecture": "福岡県", "city": "福津市", "neighborhood": "日蒔野", "banchi": "5丁目7番地の1", "postal_code": "8113298", "old_code": "81132", "post_office": "福間", "type": "office", "multiple": false, "new": false, "prefecture_kana": "フクオカケン", "city_kana": "フクツシ", "neighborhood_kana": "ヒマキノ", "alternates": []}');
@@ -141608,19 +141651,20 @@
 INSERT INTO office_data VALUES('8608513','{"jis": "43101", "kana": "クマモトチホウサイバンシヨ", "name": "熊本地方裁判所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "京町", "banchi": "1丁目13-11", "postal_code": "8608513", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "キョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608534','{"jis": "43101", "kana": "クマモトニシネンキンジムシヨ", "name": "熊本西年金事務所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "千葉城町", "banchi": "2-37", "postal_code": "8608534", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "チバジョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608739','{"jis": "43101", "kana": "クマモトワイエムシ-エ-", "name": "熊本ＹＭＣＡ", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "新町", "banchi": "1丁目3-8", "postal_code": "8608739", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "シンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608524','{"jis": "43101", "kana": "コウエキザイダンホウジン ニホンムセンキヨウカイ キユウシユウシブ", "name": "公益財団法人　日本無線協会　九州支部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "6-7いちご熊本ビル", "postal_code": "8608524", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608530','{"jis": "43101", "kana": "サンリブシテイクマナン", "name": "サンリブシティくまなん", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "平成", "banchi": "3丁目23-30", "postal_code": "8608530", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヘイセイ", "alternates": []}');
 INSERT INTO office_data VALUES('8608650','{"jis": "43101", "kana": "ザイダンホウジン カンイホケンカニユウシヤキヨウカイ キユウシユウチホウホンブ", "name": "財団法人　簡易保険加入者協会　九州地方本部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水道町", "banchi": "3-37九特会館2階", "postal_code": "8608650", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイドウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608587','{"jis": "43101", "kana": "スミトモセイメイホケン ソウゴガイシヤ クマモトシシヤ", "name": "住友生命保険　相互会社　熊本支社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "9番24号", "postal_code": "8608587", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('8608502','{"jis": "43101", "kana": "ゼンコクケンコウホケンキヨウカイ クマモトシブ", "name": "全国健康保険協会　熊本支部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5-1日本生命熊本ビル10階", "postal_code": "8608502", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608526','{"jis": "43101", "kana": "ソンガイホケンジヤパンニツポンコウア カブシキカイシヤ", "name": "損害保険ジャパン日本興亜　株式会社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "10-26", "postal_code": "8608526", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608618','{"jis": "43101", "kana": "チユオウクヤクシヨ", "name": "中央区役所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "手取本町", "banchi": "1番1号", "postal_code": "8608618", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "テトリホンチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608521','{"jis": "43101", "kana": "ツルハラヨシイ カブシキガイシヤ", "name": "鶴原吉井　株式会社", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "世安町", "banchi": "356", "postal_code": "8608521", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヨヤスマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608504','{"jis": "43101", "kana": "テルウエルニシニホン (カブ) キユウシユウシテン ナカキユウシユウエイギヨウシテン", "name": "テルウェル西日本　（株）　九州支店　中九州営業支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "南熊本", "banchi": "5丁目1-1", "postal_code": "8608504", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ミナミクマモト", "alternates": []}');
-INSERT INTO office_data VALUES('8608581','{"jis": "43101", "kana": "ニツシンイリヨウシヨクヒン カブシキカイシヤ ミナミキユウシユウシテン", "name": "日清医療食品　株式会社　南九州支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5番1号日本生命熊本ビル9階", "postal_code": "8608581", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('8608581','{"jis": "43101", "kana": "ニツシンイリヨウシヨクヒン カブシキカイシヤ ミナミキユウシユウシテン", "name": "日清医療食品　株式会社　南九州支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "辛島町", "banchi": "5番1号日本生命熊本ビル9階", "postal_code": "8608581", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "カラシマチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608602','{"jis": "43101", "kana": "ニツポンホウソウキヨウカイ クマモトホウソウキヨク", "name": "日本放送協会　熊本放送局", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "5-1", "postal_code": "8608602", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8628793','{"jis": "43101", "kana": "ニホンユウビン カブシキガイシヤ キユウシユウシシヤ ユウビンジギヨウホンブ (サンシユ)", "name": "日本郵便　株式会社　九州支社　郵便事業本部　（三種）", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "城東町", "banchi": "1-1", "postal_code": "8628793", "old_code": "860  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ジョウトウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608510','{"jis": "43101", "kana": "フジツウ カブシキガイシヤ クマモトシテン", "name": "富士通　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "紺屋今町", "banchi": "9-6", "postal_code": "8608510", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "コウヤイママチ", "alternates": []}');
 INSERT INTO office_data VALUES('8608517','{"jis": "43101", "kana": "ホテルメルパルククマモト", "name": "ホテルメルパルク熊本", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水道町", "banchi": "14-1", "postal_code": "8608517", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイドウチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608512','{"jis": "43101", "kana": "ラクテンケイシ- カブシキガイシヤ クマモトシテン", "name": "楽天ＫＣ　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "花畑町", "banchi": "12-28日本生命熊本第2ビル4F", "postal_code": "8608512", "old_code": "860  ", "post_office": "熊本中央", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ハナバタチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8608622','{"jis": "43101", "kana": "カブシキガイシヤ エヌシ-クマモト", "name": "株式会社　エヌシーくまもと", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "坪井", "banchi": "2丁目2-42(熊本中央郵便局私書箱第157号)", "postal_code": "8608622", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ツボイ", "alternates": []}');
 INSERT INTO office_data VALUES('8608611','{"jis": "43101", "kana": "カブシキガイシヤ クマモトホウソウ", "name": "株式会社　熊本放送", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "山崎町", "banchi": "30(熊本中央郵便局私書箱第87号)", "postal_code": "8608611", "old_code": "86091", "post_office": "熊本中央", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "ヤマサキマチ", "alternates": []}');
@@ -141648,15 +141692,14 @@
 INSERT INTO office_data VALUES('8628610','{"jis": "43101", "kana": "クマモトケン ケイサツホンブ", "name": "熊本県　警察本部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目18-1", "postal_code": "8628610", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628609','{"jis": "43101", "kana": "クマモトケンキヨウイクチヨウ", "name": "熊本県教育庁", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目18-1", "postal_code": "8628609", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628571','{"jis": "43101", "kana": "クマモトケンケンオウコウイキホンブゼイムブ", "name": "熊本県県央広域本部税務部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目18-1", "postal_code": "8628571", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628612','{"jis": "43101", "kana": "クマモトケンリツトシヨカン", "name": "熊本県立図書館", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "出水", "banchi": "2丁目5-1", "postal_code": "8628612", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "イズミ", "alternates": []}');
 INSERT INTO office_data VALUES('8628620','{"jis": "43101", "kana": "クマモトシスイドウキヨク", "name": "熊本市水道局", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目2-45", "postal_code": "8628620", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628688','{"jis": "43101", "kana": "クマモトロウドウキジユンカントクシヨ", "name": "熊本労働基準監督署", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "3丁目1-53", "postal_code": "8628688", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": []}');
 INSERT INTO office_data VALUES('8628666','{"jis": "43101", "kana": "スミトモカイジヨウカサイホケン カブシキガイシヤ クマモトシテン", "name": "住友海上火災保険　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "新屋敷", "banchi": "1丁目5-1", "postal_code": "8628666", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "シンヤシキ", "alternates": []}');
-INSERT INTO office_data VALUES('8628520','{"jis": "43101", "kana": "ゼンコクケンコウホケンキヨウカイ クマモトシブ", "name": "全国健康保険協会　熊本支部", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "1丁目20-22水前寺センタービル", "postal_code": "8628520", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628585','{"jis": "43101", "kana": "ニシニホンデンシンデンワ カブシキガイシヤ クマモトシテン", "name": "西日本電信電話　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "九品寺", "banchi": "1-2-11", "postal_code": "8628585", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "クホンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8628794','{"jis": "43101", "kana": "ニツポンユウセイ カブシキガイシヤ キヨウツウジムカンリジムシヨ", "name": "日本郵政　株式会社　共通事務管理事務所", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "3-1-66", "postal_code": "8628794", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": [{"jis": "43101", "kana": "ニツポンユウセイスタツフ カブシキガイシヤ キユウシユウビ-ピ-オ-センタ-", "name": "日本郵政スタッフ　株式会社　九州ＢＰＯセンター", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "大江", "banchi": "3-1-66", "postal_code": "8628794", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "オオエ", "alternates": []}]}');
 INSERT INTO office_data VALUES('8628651','{"jis": "43101", "kana": "ミツイカイジヨウカサイホケン カブシキガイシヤ クマモトシテン", "name": "三井海上火災保険　株式会社　熊本支店", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "新屋敷", "banchi": "1丁目5-1", "postal_code": "8628651", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "シンヤシキ", "alternates": []}');
 INSERT INTO office_data VALUES('8628603','{"jis": "43101", "kana": "ユウシンカンコウトウガツコウ", "name": "湧心館高等学校", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "出水", "banchi": "4丁目1-2", "postal_code": "8628603", "old_code": "862  ", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "イズミ", "alternates": []}');
 INSERT INTO office_data VALUES('8628570','{"jis": "43101", "kana": "クマモトケンチヨウ", "name": "熊本県庁", "prefecture": "熊本県", "city": "熊本市中央区", "neighborhood": "水前寺", "banchi": "6丁目18-1", "postal_code": "8628570", "old_code": "86270", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシチュウオウク", "neighborhood_kana": "スイゼンジ", "alternates": []}');
 INSERT INTO office_data VALUES('8612192','{"jis": "43102", "kana": "クマモトケン チクサンノウギヨウキヨウドウクミアイレンゴウカイ", "name": "熊本県　畜産農業協同組合連合会", "prefecture": "熊本県", "city": "熊本市東区", "neighborhood": "桜木", "banchi": "6丁目3-54", "postal_code": "8612192", "old_code": "86121", "post_office": "熊本東", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシヒガシク", "neighborhood_kana": "サクラギ", "alternates": []}');
 INSERT INTO office_data VALUES('8618514','{"jis": "43102", "kana": "クマモトカジツノウギヨウキヨウドウクミアイレンゴウカイ", "name": "熊本果実農業協同組合連合会", "prefecture": "熊本県", "city": "熊本市東区", "neighborhood": "小山町", "banchi": "1846", "postal_code": "8618514", "old_code": "862  ", "post_office": "熊本北", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシヒガシク", "neighborhood_kana": "オヤママチ", "alternates": []}');
@@ -141710,15 +141753,15 @@
 INSERT INTO office_data VALUES('8615598','{"jis": "43105", "kana": "クマモトホケンカガクダイガク", "name": "熊本保健科学大学", "prefecture": "熊本県", "city": "熊本市北区", "neighborhood": "和泉町", "banchi": "325", "postal_code": "8615598", "old_code": "86155", "post_office": "北部", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "クマモトシキタク", "neighborhood_kana": "イズミマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668686','{"jis": "43202", "kana": "カブシキガイシヤコウジンヤツシロコウジヨウ", "name": "株式会社　興人　八代工場", "prefecture": "熊本県", "city": "八代市", "neighborhood": "興国町", "banchi": "1-1(八代郵便局私書箱第22号)", "postal_code": "8668686", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "コウコクマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668502','{"jis": "43202", "kana": "ガツコウホウジン ヤツシヨウガクエンナカキユウシユウタンキダイガク", "name": "学校法人　八商学園中九州短期大学", "prefecture": "熊本県", "city": "八代市", "neighborhood": "平山新町", "banchi": "4438", "postal_code": "8668502", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ヒラヤマシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668555','{"jis": "43202", "kana": "クマモトケンヤツシロジムシヨ", "name": "熊本県八代事務所", "prefecture": "熊本県", "city": "八代市", "neighborhood": "西片町", "banchi": "1660", "postal_code": "8668555", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ニシカタマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668501','{"jis": "43202", "kana": "クマモトコウトウセンモンガツコウ ヤツシロキヤンパス", "name": "熊本高等専門学校　八代キャンパス", "prefecture": "熊本県", "city": "八代市", "neighborhood": "平山新町", "banchi": "2627", "postal_code": "8668501", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ヒラヤマシンマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668585','{"jis": "43202", "kana": "クマモトチホウサイバンシヨヤツシロシブ・ヤツシロカンイサイバンシヨ", "name": "熊本地方裁判所八代支部・八代簡易裁判所", "prefecture": "熊本県", "city": "八代市", "neighborhood": "西松江城町", "banchi": "1-41", "postal_code": "8668585", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ニシマツエジョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668510','{"jis": "43202", "kana": "シライシセイカカブシキカイシヤ", "name": "白石製菓　株式会社", "prefecture": "熊本県", "city": "八代市", "neighborhood": "新浜町", "banchi": "1-1-28", "postal_code": "8668510", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "シンハママチ", "alternates": []}');
-INSERT INTO office_data VALUES('8668660','{"jis": "43202", "kana": "ドクリツギヨウセイホウジン チイキイリヨウキノウスイシンキコウ クマモトソウゴウビヨウイン", "name": "独立行政法人　地域医療機能推進機構　熊本総合病院", "prefecture": "熊本県", "city": "八代市", "neighborhood": "通町", "banchi": "10-10(八代郵便局私書箱第19号)", "postal_code": "8668660", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": true, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "トオリチョウ", "alternates": []}');
+INSERT INTO office_data VALUES('8668660','{"jis": "43202", "kana": "ドクリツギヨウセイホウジン チイキイリヨウキノウスイシンキコウ クマモトソウゴウビヨウイン", "name": "独立行政法人　地域医療機能推進機構　熊本総合病院", "prefecture": "熊本県", "city": "八代市", "neighborhood": "通町", "banchi": "10-10(八代郵便局私書箱第19号)", "postal_code": "8668660", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "トオリチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8668533','{"jis": "43202", "kana": "ドクリツギヨウセイホウジン ロウドウシヤケンコウフクシキコウ クマモトロウサイビヨウイン", "name": "独立行政法人　労働者健康福祉機構　熊本労災病院", "prefecture": "熊本県", "city": "八代市", "neighborhood": "竹原町", "banchi": "1670", "postal_code": "8668533", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "タケハラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668602','{"jis": "43202", "kana": "ニツポンセイシカブシキガイシヤヤツシロコウジヨウ", "name": "日本製紙　株式会社　八代工場", "prefecture": "熊本県", "city": "八代市", "neighborhood": "十条町", "banchi": "1-1(八代郵便局私書箱第13号)", "postal_code": "8668602", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ジュウジョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668503','{"jis": "43202", "kana": "ヤツシロシヤカイホケンジムシヨ", "name": "八代社会保険事務所", "prefecture": "熊本県", "city": "八代市", "neighborhood": "萩原町", "banchi": "2丁目11-41", "postal_code": "8668503", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ハギワラマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668601','{"jis": "43202", "kana": "ヤツシロシヤクシヨ", "name": "八代市役所", "prefecture": "熊本県", "city": "八代市", "neighborhood": "松江城町", "banchi": "1-25(八代郵便局私書箱第1号)", "postal_code": "8668601", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "マツエジョウマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8668605','{"jis": "43202", "kana": "ヤツシロゼイムシヨ", "name": "八代税務署", "prefecture": "熊本県", "city": "八代市", "neighborhood": "花園町", "banchi": "16-2(八代郵便局私書箱第26号)", "postal_code": "8668605", "old_code": "866  ", "post_office": "八代", "type": "box", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "ハナゾノチョウ", "alternates": []}');
 INSERT INTO office_data VALUES('8668511','{"jis": "43202", "kana": "ワイケイケイカブシキカイシヤキユウシユウコウジヨウ", "name": "ＹＫＫ　株式会社　九州工場", "prefecture": "熊本県", "city": "八代市", "neighborhood": "新港町", "banchi": "1丁目10", "postal_code": "8668511", "old_code": "866  ", "post_office": "八代", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "シンミナトマチ", "alternates": []}');
 INSERT INTO office_data VALUES('8694292','{"jis": "43202", "kana": "ヤツシロシ カガミシシヨ", "name": "八代市　鏡支所", "prefecture": "熊本県", "city": "八代市", "neighborhood": "鏡町内田", "banchi": "453番地1", "postal_code": "8694292", "old_code": "86942", "post_office": "鏡", "type": "office", "multiple": false, "new": false, "prefecture_kana": "クマモトケン", "city_kana": "ヤツシロシ", "neighborhood_kana": "カガミマチウチダ", "alternates": []}');
```

### Comparing `posuto-2023.7.0/posuto/posuto.py` & `posuto-2023.8.0/posuto/posuto.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/posuto/prep.py` & `posuto-2023.8.0/posuto/prep.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/posuto/tests/test_basic.py` & `posuto-2023.8.0/posuto/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.7.0/posuto.egg-info/PKG-INFO` & `posuto-2023.8.0/posuto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -37,17 +37,19 @@
 <img src="https://github.com/polm/posuto/raw/master/postcharacter.png" width=125 height=125 alt="Postbox character by Irasutoya" />
 
 Features:
 
 - multi-line neighborhoods are joined
 - parenthetical notes are put in a separate field
 - change reasons are converted from flags to labels
-- romaji and kana records are unified for easy access
+- kana records are unified for easy access
 - codes with multiple areas provide a list of alternates
 
+Romaji provided by JP Post were previously included in this library, but they are extremely low quality and hard to sync, due to being updated separately. If you need romaji it is recommended you use [cutlet](https://github.com/polm/cutlet) instead.
+
 To install:
 
     pip install posuto
 
 Example usage:
 
     import posuto as 〒
@@ -56,16 +58,14 @@
 
     print(🗼)
     # "東京都港区芝公園"
     print(🗼.prefecture)
     # "東京都"
     print(🗼.kana)
     # "トウキョウトミナトクシバコウエン"
-    print(🗼.romaji)
-    # "Tokyo To, Minato Ku, Shibakoen"
     print(🗼.note)
     # None
 
 **Note:** Unfortunately 〒 and 🗼 are not valid identifiers in Python, so the
 above is pseudocode. See [examples/sample.py][] for an executable version.
 
 [examples/sample.py]: https://github.com/polm/posuto/blob/master/examples/sample.py
```

### Comparing `posuto-2023.7.0/setup.cfg` & `posuto-2023.8.0/setup.cfg`

 * *Files identical despite different names*

